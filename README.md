<div align="center">

<img src="https://raw.githubusercontent.com/kirukayu/kirukayu/main/media/banner.gif" width="100%" alt="londo">

<br><br>

<img src="https://raw.githubusercontent.com/kirukayu/kirukayu/main/media/langs.png" height="58" alt="lua, rust, typescript, python, c++, java">

<br><br>

<img src="https://raw.githubusercontent.com/kirukayu/kirukayu/main/media/stack.png" height="48" alt="react, vite, tauri, electron, node, astro, fastapi, qt">

<br><br>

<img src="https://raw.githubusercontent.com/kirukayu/kirukayu/main/media/tools.png" height="48" alt="blender, roblox studio, git">

</div>

<br>

i build tools for games. launchers, runtime tooling, and the reverse engineering
that comes first.

**luau** is my main language: roblox runtime tooling, ui libraries, bytecode and
obfuscator output. **rust** holds anything that must not lose data. **typescript**
for interfaces. python, c++ and java where they fit.

<br>

---

<br>

### roundtable

<div align="center">

<img src="https://raw.githubusercontent.com/kirukayu/kirukayu/main/media/roundtable.gif" width="740" alt="the roundtable interface">

</div>

mod, co-op and save management for elden ring and the rest of fromsoftware's
catalogue.

it parses the `.sl2` save container, so moving a character to another account
rewrites the steam id in place and recomputes the md5 checksums the game checks
on load. it reads modengine 2 and me3 config, picks the loader chain that will
actually start your copy, and shows that plan first.

the window runs a server on loopback and opens your browser at it. rust and axum
below, react and motion above.
