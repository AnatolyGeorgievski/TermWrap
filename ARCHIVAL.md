# Archival fork

Срез для lab: рабочая копия `llccd/TermWrap`, чтобы не потерять код, если upstream уйдёт в private или исчезнет.

- Upstream: https://github.com/llccd/TermWrap
- Дата среза: 2026-11-02
- Намерение: **хранить**, не вести свой rewrite. Обновления — `git fetch upstream` по нужде.
- Lab-канон рядом: Pro + native RDP + UIA bridge; этот wrap — только Home-bootstrap.

## Build

- Lab installs **prebuilt** release `archive/2026-11-02-bin` (see mcp-rdp-lab).
- To rebuild from this tree: **Visual Studio / MSBuild (MSVC v143)** — upstream is `.vcxproj`.
- **Not** MinGW/MSYS2 makefile for the ServiceDll (svchost / msvcrt link model).

Тег среза: `archive/2026-11-02`.
