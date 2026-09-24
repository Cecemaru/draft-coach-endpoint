# draft-coach-endpoint

One file: `endpoint.json`, which says where the Draft Coach engine is answering right now.

`DraftCoach.exe` reads it on startup. The tunnel in front of the engine gets a new address every time it
restarts, so the exe cannot hold one; it holds the address of *this file* instead, and this file never moves.

Nothing else lives here. The engine, the data and the source are somewhere else.
