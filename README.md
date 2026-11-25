# hunterr

A small, AI-first service that searches the *arr backlog: it finds missing episodes and movies and asks Sonarr and Radarr to look for them.

## Why

Sonarr and Radarr don't go back and search for things that have been missing for a while. After an item is added they only watch RSS for new releases, so anything that failed or was skipped stays missing until someone searches by hand. Huntarr used to cover that gap until it was dropped over security problems. hunterr is meant to replace it:

- **No web UI.** An AI agent is the main way to run it and to check that the hunt loop is working.
- **Sonarr and Radarr make the decisions.** hunterr only chooses *what* to search and *when*. It never picks releases itself.
- **Small attack surface.** API keys never leave the service, and nothing is reachable without authentication.

## Status

In design, nothing built yet. Design docs will go in `docs/`.

## License

[MIT](LICENSE)
