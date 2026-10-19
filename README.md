<!-- ffxiv-tc-port 繁體中文說明開始 -->
# cimguizmo(台服 fork)

ImGuizmo（Dear ImGui 的 3D 操作軸元件）的 C API 綁定（上游 [goatcorp/gc-cimguizmo](https://github.com/goatcorp/gc-cimguizmo)，再往上是 [cimgui/cimguizmo](https://github.com/cimgui/cimguizmo)）。Dalamud 本體把它編成 `cimguizmo.dll`。

## 台服 fork 的目的

- 讓 Dalamud 本體與這裡的子模組 `ImGuizmo` 都指向本 org，建置不依賴上游 repo 是否還在、有沒有被改寫。

## 與上游的差異

- 子模組 `ImGuizmo` 的網址改指 [ffxiv-tc-port/gc-ImGuizmo](https://github.com/ffxiv-tc-port/gc-ImGuizmo)。原始碼與上游相同。
- 本分支 `tc-submodule-url` 建在上游較早的 `master` 上，上游之後的更新沒有合入。

## 誰在用它

- [Dalamud](https://github.com/ffxiv-tc-port/Dalamud)：子模組 `lib/cimguizmo`。

---

以下為上游原始 README，內容未經修改：

<!-- ffxiv-tc-port 繁體中文說明結束 -->
# cimguizmo

This is a c-api wrapper for ImGuizmo (https://github.com/CedricGuillemet/ImGuizmo)  which is a guizmo for Dear ImGui (https://github.com/ocornut/imgui)

ImGuizmo is a submodule of this repo. To do generation again in case ImGuizmo is changed, you should update ImGuizmo, make sure that cimgui repository is a sibling folder to this repository folder and execute generator/generator.bat(.sh)
