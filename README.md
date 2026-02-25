# MosaicRemoverExtension (White_1.0 / BepInEx)

日本語 / 中文 / English

## 日本語

### 概要

- 表現の修正
- 男キャラ系アセットの非表示（複数男シチュ対応の判定強化済み）
- ズーム強化（FOV拡張）
- FreeCam（マウス中心操作）
- ポイント加算 / ポイント獲得倍率

### 導入
前提:

- `BepInEx 5.x` 導入済み

配置:

- `BepInEx/plugins/MosaicRemoverExtension.dll`

設定ファイル（初回起動後に生成）:

- `BepInEx/config/com.bepinex.plugin.mosaicremover.extension.cfg`

### デフォルトキー

- `F5`: ポイント加算（+1000）
- `F6`: FreeCam ON/OFF
- `F7`: 男キャラアセット非表示 ON/OFF
- `F8`: ズーム強化 ON/OFF
- `Home`: ズーム（FOV）リセット
- `R`: FreeCam中に女キャラ付近へスナップ（見つからない場合はFreeCamリセット）
- `F12`: 右下の小さい状態表示 ON/OFF

### FreeCam操作（現在の推奨）

- `RMB + ドラッグ`: 回転
- `LMB + ドラッグ`: 平行移動（XY）
- `RMB + ホイール`: 前後移動（Z / ドリー）
- `ホイールのみ`: FOVズーム（F8有効時）
- `MMB + ドラッグ`: 平行移動（XY）

補助操作（任意）:

- `RMB + WASD/QE`: XYZ移動

### 主な設定項目

- `[MaleAssetHider] NameKeywords`
- `[ZoomEnhancer] MinFov / MaxFov / WheelStepFov`
- `[FreeCam] OrbitSensitivity / PanSensitivity / DollySensitivity / MoveSpeed`
- `[FreeCam] BlockInputOverUI`
- `[PointCheat] PointGainMultiplier / AddPointsAmount`
- `[General] SceneWhitelist`

### 注意事項（重要）

- FreeCam は「FreeCam前提で使う」運用を推奨しています。
- シーンによっては `F6` で FreeCam をOFFにした際、ゲーム側カメラ制御の影響で視点がずれる場合があります。
- 視点を見失ったら `R`（女キャラ付近へスナップ）を使ってください。

---

## 中文（简体）

### 概述

- 隐藏男性角色相关资产（已增强多男性场景识别）
- 强化缩放（FOV）
- FreeCam（以鼠标操作为主）
- 点数增加 / 点数获取倍率

### 安装
前提：

- 已安装 `BepInEx 5.x`

放置：

- `BepInEx/plugins/MosaicRemoverExtension.dll`

配置文件（首次启动后生成）：

- `BepInEx/config/com.bepinex.plugin.mosaicremover.extension.cfg`

### 默认按键

- `F5`: 增加点数（+1000）
- `F6`: FreeCam 开/关
- `F7`: 隐藏男性资产 开/关
- `F8`: 缩放增强 开/关
- `Home`: 重置缩放（FOV）
- `R`: FreeCam中跳到女角色附近（找不到则执行FreeCam重置）
- `F12`: 右下角状态小字显示 开/关

### FreeCam 操作（推荐）

- `右键 + 拖动`: 旋转
- `左键 + 拖动`: 平移（XY）
- `右键 + 滚轮`: 前后移动（Z / Dolly）
- `仅滚轮`: FOV缩放（需 F8 开启）
- `中键 + 拖动`: 平移（XY）

可选辅助操作：

- `右键 + WASD/QE`: XYZ移动

### 常用配置项

- `[MaleAssetHider] NameKeywords`
- `[ZoomEnhancer] MinFov / MaxFov / WheelStepFov`
- `[FreeCam] OrbitSensitivity / PanSensitivity / DollySensitivity / MoveSpeed`
- `[FreeCam] BlockInputOverUI`
- `[PointCheat] PointGainMultiplier / AddPointsAmount`
- `[General] SceneWhitelist`

### 注意事项（重要）

- 建议按“以 FreeCam 为主”的方式使用。
- 某些场景下关闭 FreeCam（`F6`）时，可能会受到游戏原生相机逻辑影响而出现视角偏移。
- 如果镜头丢失目标，请按 `R` 快速跳回女角色附近。

---

## English

### Overview

- Male asset hiding (with improved detection for multi-male scenes)
- Enhanced zoom (FOV)
- FreeCam (mouse-focused controls)
- Point add / point gain multiplier

### Installation
Requirements:

- `BepInEx 5.x` installed

Place:

- `BepInEx/plugins/MosaicRemoverExtension.dll`

Config file (generated after first launch):

- `BepInEx/config/com.bepinex.plugin.mosaicremover.extension.cfg`

### Default Hotkeys

- `F5`: Add points (+1000)
- `F6`: Toggle FreeCam
- `F7`: Toggle male asset hide
- `F8`: Toggle zoom enhancer
- `Home`: Reset zoom (FOV)
- `R`: Snap near female character in FreeCam (falls back to FreeCam reset if not found)
- `F12`: Toggle small status overlay (bottom-right)

### FreeCam Controls (Recommended)

- `RMB + Drag`: Rotate
- `LMB + Drag`: Pan (XY)
- `RMB + Wheel`: Move forward/backward (Z / dolly)
- `Wheel only`: FOV zoom (when F8 is ON)
- `MMB + Drag`: Pan (XY)

Optional helper controls:

- `RMB + WASD/QE`: XYZ movement

### Useful Config Options

- `[MaleAssetHider] NameKeywords`
- `[ZoomEnhancer] MinFov / MaxFov / WheelStepFov`
- `[FreeCam] OrbitSensitivity / PanSensitivity / DollySensitivity / MoveSpeed`
- `[FreeCam] BlockInputOverUI`
- `[PointCheat] PointGainMultiplier / AddPointsAmount`
- `[General] SceneWhitelist`

### Notes (Important)

- Recommended usage is “FreeCam-first”.
- In some scenes, turning FreeCam OFF (`F6`) may still be affected by the game’s native camera logic and cause a view shift.
- If you lose the view target, press `R` to snap back near the female character.

