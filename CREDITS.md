# Credits and dependency provenance

- **Universal Modder 0.2.0**: installed plugin used for game reconnaissance, reverse-engineering workflow, backups and original-game automation. Project implementation and testing were AI-assisted in Codex.
- **Khronos OpenXR-SDK**, Apache 2.0. Commit `f2448a8797c85814aa892efc1ab8707900fbcc78`. Static native Windows x86 loader and headers. [Official source](https://github.com/KhronosGroup/OpenXR-SDK). License: `licenses/OpenXR-SDK.txt`.
- **Tsuda Kageyu's MinHook**, BSD-style license. Commit `8af6b4acae5a9388fd742b56fa79ece89d96f823`. Native hook/trampoline library. [Official source](https://github.com/TsudaKageyu/minhook). License: `licenses/MinHook.txt`.
- **DJ Lynch's bo1-vr**, MIT. Commit `4450927118c6baf7a023da6967d77e0e745de193`. Prior renderer/coordinate investigation reference. Its OpenVR/Linux/Proton approach is not the Windows/OpenXR implementation delivered here. [Reference project](https://github.com/daniel-lynch/bo1-vr). License retained at `licenses/bo1-vr-reference.txt`.
- **Nukem9/LinkerMod**. Commit `72ee05bbf42dfb2a1893e655788b631be63ea317`. Public original-game modding and structure-metadata reference, independently checked against the user's executable and runtime. Its loader, broader patches and authentication modifications are not included. [Reference project](https://github.com/Nukem9/LinkerMod).

- **Scobalula/Greyhound**. Public native model/skin-layout metadata reference, checked against loaded BO1 data. No exporter code or original exported meshes are included. [Reference project](https://github.com/Scobalula/Greyhound).

Call of Duty: Black Ops and its original content belong to their respective owners. This extension requires the user's installed game and includes no original executables, maps, models, textures, scripts, audio or decompiled engine source.

OpenXR session/swapchain lifecycle follows the [Khronos specification](https://registry.khronos.org/OpenXR/specs/1.1/html/xrspec.html). The implementation preserves the original D3D9 game and uses OpenXR's PC D3D11 graphics binding for submission.

Implementation and testing are AI-assisted with OpenAI Codex (GPT-6 family).

- **nlohmann/json 3.12.0**, MIT. Used by the local pose importer and validated runtime profile reader. License: `licenses/nlohmann-json-MIT.txt`. The user-authored Pose Studio format and poses remain separate personal data.
