<div align="center">

<img src="https://raw.githubusercontent.com/kirukayu/kirukayu/main/media/banner.gif" width="100%" alt="londo">

<br><br>

<img src="https://raw.githubusercontent.com/kirukayu/kirukayu/main/media/langs.png" height="62" alt="lua, rust, typescript, python, c++, java">

<br><br>

<img src="https://raw.githubusercontent.com/kirukayu/kirukayu/main/media/stack.png" height="52" alt="react, vite, tauri, electron, node, astro, fastapi, qt">

<br><br>

<img src="https://raw.githubusercontent.com/kirukayu/kirukayu/main/media/tools.png" height="52" alt="blender, roblox studio, git">

</div>

<br>

i build tools for games — launchers, runtime tooling, and the reverse engineering
that has to happen first. mostly windows, mostly at the layer where a program and
the thing it is talking to disagree about what is allowed.

<br>

**luau / lua** is my first language and still the one i reach for. roblox runtime
tooling, ui libraries, and reading code that did not want to be read — bytecode,
obfuscator output, and the small utilities that make both tractable.

**rust** is where the parts that must not lose data live: binary formats,
filesystem work, local http services, tauri backends. **typescript** for
interfaces, with a real interest in motion — the difference between a page that
works and a page that feels built is about four hundred milliseconds. **python**
for desktop apps and analysis tooling, **c++** when nothing above it will do, and
**java** for minecraft server plugins.

reverse engineering: lua and luau bytecode, vm-based obfuscators, binary container
formats, and anti-cheat behaviour — the analysis side of it, so that tooling can be
built against something known rather than guessed at.

<br>

---

<br>

### roundtable

<div align="center">

<img src="https://raw.githubusercontent.com/kirukayu/kirukayu/main/media/roundtable.gif" width="760" alt="the roundtable interface">

</div>

mod, co-op and save management for elden ring and every other fromsoftware title.

three things that should be simple are not: running a large overhaul alongside
seamless co-op, starting a modded game on a copy that did not come from steam, and
moving a character between installations that use different account ids. each has a
known answer, and none of them is one click. this makes them one click.

it reads the `.sl2` save container directly — transferring a character means
rewriting every occurrence of the account id and recomputing the md5 checksums the
game verifies. it reads modengine 2 and me3 configuration, works out which loader
chain will actually start a given installation, and shows you that plan before it
runs it.

the window does not draw the interface. it starts a server on loopback and hands the
address to your browser, then stays alive to serve the folder dialogs a browser
cannot open. rust and axum underneath, react and motion on top.

<br>

---

<br>

<div align="center">
<sub>everything here runs locally. no telemetry, no analytics, no account.</sub>
</div>
