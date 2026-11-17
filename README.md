# tester — 小到离谱，自由到离谱。

**A minimal VRChat avatar. Maximum freedom. CC0.**

[简体中文](#简体中文) · [English](#english) · [日本語](#日本語)

**[下载 / Download / ダウンロード：tester.unitypackage](https://github.com/donywang922/tester/releases/latest/download/tester.unitypackage)** · [Releases](https://github.com/donywang922/tester/releases)

**2,171 triangles · 53 bones · 18 blendshapes · 1 mesh · 1 material · CC0**

---

## 简体中文

### 什么？！完整人形骨架，打包带走，连署名都不用？！

**没错。售价：0。署名要求：0。额外插件依赖：0。**

这就是 **tester**：一个把“最简”贯彻到底的 VRChat Avatar。一个模型，一套完整的 VRC 人形骨架，该有的基础能力都有，多余部件一个不带。拿来测试、拿来展示、拿来改造，甚至直接塞进你的插件发布包——**随便用，不用问，什么都不用声明。**

### 体积精简，基础配置直接给满！

- **极简本体。** 单网格、单材质，无额外服装、饰品、挂件、粒子或花哨功能系统。
- **完整 VRC 人形骨架。** 躯干、头颈、肩膀、四肢、双手全部手指和脚趾骨骼齐备，另带双眼骨骼；已配置 Unity Humanoid。
- **开口就能测。** 15 个 VRC 口型 BlendShape，预制体已配置 Viseme Lip Sync。
- **眼睛也没落下。** 已配置 Eye Look，以及闭眼、向上看、向下看的眼睑 BlendShape。
- **额外依赖？零。** 除 Unity 和官方 VRChat SDK 外，无需另装第三方 Shader、插件或运行库。材质使用 SDK 自带的 `VRChat/Mobile/Toon Standard`。

### 版权与使用：CC0，直接拿走！

本项目自制模型资产以 **CC0 1.0 Universal** 公开，没有额外的版权授权门槛。免费使用、修改、复制、商用、再分发，都可以。

**无需署名，无需注明来源，无需附上本 README，无需发布使用声明，也无需事先征求许可。**

你可以用它做插件测试、自动化测试、动画与骨骼验证、教程、截图、视频、直播、商品演示、展示用 Avatar，或者直接随免费或收费插件、工具、示例工程一起发布。原样带走可以，改完再发也可以。

本项目自制资产的许可全文见 [LICENSE](LICENSE)。Unity、VRChat SDK 及其他第三方软件仍适用各自的许可。

### 规格表：数字也很能打。

| 项目 | 参数 |
| --- | --- |
| 模型文件 | `Assets/tester merged.fbx` |
| 预制体 | `Assets/tester merged.prefab` |
| 网格 / Skinned Mesh Renderer | 1 / 1 |
| 材质 | 1：`Assets/toon lit.mat` |
| Shader | `VRChat/Mobile/Toon Standard`，官方 SDK 自带 |
| 自定义贴图 | 0；材质另引用 SDK 自带的阴影 Ramp |
| FBX 源顶点数 | 2,299 |
| FBX 源多边形数 | 2,141 |
| 三角化后面数 | **2,171** |
| 骨骼 | **53**：51 根已映射的 Humanoid 骨骼 + 2 根眼骨 |
| 手指骨骼 | 30：双手各 5 指，每指 3 节 |
| BlendShape | **18**：15 个口型 + `EyesClosed`、`LookUp`、`LookDown` |
| 口型 / 眼神 / 眼睑 | 预制体中已配置 |
| 视点高度 | 约 1.003 m，Avatar Descriptor 本地 Y 坐标 |
| PhysBones / Contacts / 粒子系统 | 0 / 0 / 0 |
| 自定义动画控制器 / 表情菜单 / 表情参数资产 | 0 / 0 / 0；使用 SDK 默认动画层 |
| 自定义脚本 | 0；预制体仅添加官方 SDK 的 Avatar Descriptor 和 Pipeline Manager |
| FBX 文件大小 | 213,356 bytes，约 **208.4 KiB** |
| UnityPackage 大小 | 118,465 bytes，约 **115.7 KiB** |
| 项目 Unity 版本 | `2022.3.22f1` |
| 项目 VRChat SDK 版本 | Avatars / Base `3.10.5` |
| 许可 | **CC0 1.0 Universal** |

几何数据统计自当前 FBX；Unity 导入后的顶点数可能因法线拆分等处理而不同。文件大小为磁盘文件大小，不代表上传后的 Avatar Bundle 大小。

### 三步开用！

1. 准备装有官方 VRChat Avatars SDK 的 Unity 工程。可直接打开本项目，或从 [Releases](https://github.com/donywang922/tester/releases) 下载并导入 `tester.unitypackage`；该包包含 FBX、材质和预制体。
2. 打开 `Assets/main.unity`，或把 `Assets/tester merged.prefab` 拖进场景。
3. 开始测试、展示或修改！如需上传为自己的 Avatar，请先在 Pipeline Manager 中 **Detach 现有 Blueprint ID**，再通过 SDK 上传。

本项目的开发环境安装了 Gesture Manager，**它是可选调试工具，模型和预制体不依赖它**。

**一个干净的测试模型，一整套人形骨架，零署名要求。拿去，让你的项目直接开跑！**

---

## English

### Wait. A complete humanoid rig—and you don't even need to credit anyone?!

**Correct. Price: zero. Required attribution: zero. Extra plugin dependencies: zero.**

Meet **tester**, a VRChat avatar that takes minimalism seriously. One model. A complete VRC humanoid rig. All the essentials, with no extra parts. Test with it, demo with it, modify it, or bundle it right inside your plugin release. **Use it freely. No permission request. No credit. No usage declaration.**

### Tiny package. Essentials included!

- **Minimal by design.** One mesh, one material, with no extra outfits, accessories, attachments, particles, or elaborate feature systems.
- **Complete VRC humanoid rig.** Torso, head, neck, shoulders, limbs, every finger, and toes, plus two eye bones. Unity Humanoid mapping is already configured.
- **Ready for lip-sync testing.** All 15 VRC viseme blendshapes, with Viseme Lip Sync configured in the prefab.
- **Eyes included.** Eye Look and eyelid blendshapes for closing the eyes, looking up, and looking down are configured.
- **Zero extra dependencies.** Only Unity and the official VRChat SDK are needed. No additional third-party shaders, plugins, or runtime libraries. The material uses `VRChat/Mobile/Toon Standard`, included with the SDK.

### CC0. Take it and make something!

The project's original model assets are released under **CC0 1.0 Universal**, with no additional copyright permission requirements. Use, modify, copy, commercialize, and redistribute them freely.

**No attribution. No source credit. No requirement to include this README. No usage declaration. No need to ask first.**

Use the model for plugin testing, automated tests, animation and rig checks, tutorials, screenshots, videos, streams, product demonstrations, or display avatars. Bundle it with free or paid plugins, tools, and example projects. Redistribute it unchanged or modified.

See [LICENSE](LICENSE) for the full terms covering the project's original assets. Unity, the VRChat SDK, and other third-party software remain under their respective licenses.

### The specs speak for themselves.

| Item | Specification |
| --- | --- |
| Model | `Assets/tester merged.fbx` |
| Prefab | `Assets/tester merged.prefab` |
| Meshes / Skinned Mesh Renderers | 1 / 1 |
| Materials | 1: `Assets/toon lit.mat` |
| Shader | `VRChat/Mobile/Toon Standard`, included with the official SDK |
| Custom textures | 0; the material also references an SDK shadow ramp |
| FBX source vertices | 2,299 |
| FBX source polygons | 2,141 |
| Triangles after triangulation | **2,171** |
| Bones | **53**: 51 mapped Humanoid bones + 2 eye bones |
| Finger bones | 30: 5 fingers per hand, 3 bones per finger |
| Blendshapes | **18**: 15 visemes + `EyesClosed`, `LookUp`, `LookDown` |
| Lip sync / Eye Look / Eyelids | Configured in the prefab |
| Viewpoint height | Approximately 1.003 m, Avatar Descriptor local Y coordinate |
| PhysBones / Contacts / Particle systems | 0 / 0 / 0 |
| Custom animator controllers / Expression menus / Expression parameter assets | 0 / 0 / 0; uses SDK default animation layers |
| Custom scripts | 0; the prefab only adds the official SDK Avatar Descriptor and Pipeline Manager |
| FBX file size | 213,356 bytes, approximately **208.4 KiB** |
| UnityPackage size | 118,465 bytes, approximately **115.7 KiB** |
| Project Unity version | `2022.3.22f1` |
| Project VRChat SDK version | Avatars / Base `3.10.5` |
| License | **CC0 1.0 Universal** |

Geometry counts come from the current FBX. Unity's imported vertex count may differ due to normal splitting and other import processing. File sizes are on-disk sizes, not the uploaded avatar bundle size.

### Three steps. You're in!

1. Prepare a Unity project with the official VRChat Avatars SDK. Open this project directly, or download and import `tester.unitypackage` from [Releases](https://github.com/donywang922/tester/releases). The package contains the FBX, material, and prefab.
2. Open `Assets/main.unity`, or drag `Assets/tester merged.prefab` into your scene.
3. Test, demonstrate, and customize! To upload it as your own avatar, first **Detach the existing Blueprint ID** in Pipeline Manager, then upload through the SDK.

Gesture Manager is installed in this project's development environment. **It is an optional debugging tool; the model and prefab do not depend on it.**

**One clean test model. A complete humanoid rig. Zero required credit. Grab it and get your project moving!**

---

## 日本語

### えっ？！フル人型リグ付きで、クレジット表記すら不要？！

**そのとおり。価格：0。クレジット表記の義務：0。追加プラグイン依存：0。**

**tester** は、「最小限」をとことん追求した VRChat アバターです。モデルはひとつ。VRC 用の人型リグはひと通り完備。必要な基本機能を備え、余計なパーツは一切なし。テストにも、デモにも、改変にも。あなたのプラグインに同梱して、そのまま配布しても OK！ **使用報告も、許可申請も、クレジット表記も不要です。**

### 小さくても、基本は全部入り！

- **徹底したシンプルさ。** 1 メッシュ・1 マテリアル。追加衣装、アクセサリー、装飾パーツ、パーティクル、複雑なギミックはありません。
- **VRC 用の人型リグを完備。** 胴体、頭、首、肩、四肢、両手の全指、つま先に加え、左右の目ボーンも搭載。Unity Humanoid のマッピングは設定済みです。
- **リップシンクもすぐ試せる。** VRC 用の全 15 種の Viseme BlendShape を搭載し、Prefab のリップシンクも設定済みです。
- **目の動きもお任せ。** Eye Look と、閉眼・上目・下目用のまぶた BlendShape を設定済みです。
- **追加依存はゼロ。** 必要なのは Unity と公式 VRChat SDK だけ。別途導入するサードパーティ製 Shader、プラグイン、ランタイムライブラリは不要です。マテリアルには SDK 付属の `VRChat/Mobile/Toon Standard` を使用しています。

### CC0。どうぞ、そのままお持ち帰りください！

本プロジェクトのオリジナルモデルアセットは **CC0 1.0 Universal** で公開しています。追加の著作権利用許諾は不要。使用、改変、複製、商用利用、再配布まで自由です。

**作者名の表記不要。出典の記載不要。この README の添付不要。使用報告不要。事前の許可申請も不要です。**

プラグインの動作確認、自動テスト、アニメーションやリグの検証、チュートリアル、スクリーンショット、動画、配信、商品デモ、展示用アバターなどにご利用ください。無料・有料を問わず、プラグイン、ツール、サンプルプロジェクトへの同梱配布も OK。改変してもしなくても、再配布できます。

オリジナルアセットのライセンス全文は [LICENSE](LICENSE) をご覧ください。Unity、VRChat SDK、その他のサードパーティ製ソフトウェアには、それぞれのライセンスが適用されます。

### 数字で見ても、この身軽さ。

| 項目 | 仕様 |
| --- | --- |
| モデル | `Assets/tester merged.fbx` |
| Prefab | `Assets/tester merged.prefab` |
| メッシュ / Skinned Mesh Renderer | 1 / 1 |
| マテリアル | 1：`Assets/toon lit.mat` |
| Shader | `VRChat/Mobile/Toon Standard`、公式 SDK 付属 |
| 独自テクスチャ | 0；マテリアルは SDK 付属のシャドウ Ramp も参照 |
| FBX 元データの頂点数 | 2,299 |
| FBX 元データのポリゴン数 | 2,141 |
| 三角形換算 | **2,171** |
| ボーン数 | **53**：Humanoid にマッピング済みの 51 本 + 目ボーン 2 本 |
| 指ボーン | 30 本：片手 5 指、各指 3 本 |
| BlendShape | **18**：Viseme 15 種 + `EyesClosed`、`LookUp`、`LookDown` |
| リップシンク / Eye Look / まぶた | Prefab で設定済み |
| 視点の高さ | 約 1.003 m、Avatar Descriptor のローカル Y 座標 |
| PhysBones / Contacts / パーティクルシステム | 0 / 0 / 0 |
| 独自 Animator Controller / Expression Menu / Expression Parameters アセット | 0 / 0 / 0；SDK の標準アニメーションレイヤーを使用 |
| 独自スクリプト | 0；Prefab で追加しているのは公式 SDK の Avatar Descriptor と Pipeline Manager のみ |
| FBX ファイルサイズ | 213,356 bytes、約 **208.4 KiB** |
| UnityPackage サイズ | 118,465 bytes、約 **115.7 KiB** |
| プロジェクトの Unity バージョン | `2022.3.22f1` |
| プロジェクトの VRChat SDK バージョン | Avatars / Base `3.10.5` |
| ライセンス | **CC0 1.0 Universal** |

形状の数値は現在の FBX 元データから集計しています。Unity インポート後の頂点数は、法線による頂点分割などで変わる場合があります。ファイルサイズはディスク上の値であり、アップロード後の Avatar Bundle サイズではありません。

### たった 3 ステップで使えます！

1. 公式 VRChat Avatars SDK を導入した Unity プロジェクトを用意します。このプロジェクトを直接開くか、[Releases](https://github.com/donywang922/tester/releases) から `tester.unitypackage` をダウンロードしてインポートしてください。パッケージには FBX・マテリアル・Prefab が含まれています。
2. `Assets/main.unity` を開くか、`Assets/tester merged.prefab` をシーンに配置します。
3. テストも、デモも、改変も自由にどうぞ！ 自分のアバターとしてアップロードする場合は、先に Pipeline Manager で **既存の Blueprint ID を Detach** してから、SDK でアップロードしてください。

本プロジェクトの開発環境には Gesture Manager がインストールされていますが、**任意のデバッグツールであり、モデルと Prefab の必須依存ではありません**。

**シンプルなテストモデルに、ひと通り揃った人型リグ。クレジット表記も不要。さあ、あなたのプロジェクトで使い倒してください！**
