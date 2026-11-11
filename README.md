# FilterBlade 中文补全

给 [filterblade.xyz](https://www.filterblade.xyz/?game=Poe1) 用的汉化工具，把网站界面完整中文化。

内置词典，装完即可使用，不需要任何前置汉化插件。提供 Chrome 插件和用户脚本两种形式，任选其一。

## 安装


### 方式二：用户脚本（Tampermonkey）（推荐）

1. 浏览器安装 [Tampermonkey](https://www.tampermonkey.net/)（篡改猴）
2. 点 Tampermonkey 图标 → **实用工具** → **导入** → 选 `filterblade-zh.js`
3. 在 `chrome://extensions` → 篡改猴 → **详细信息** → 页面底部打开 **允许用户脚本**
4. 刷新 filterblade

> Chrome 138 起必须打开上面那个开关，否则任何用户脚本都不会生效。

### 方式一：Chrome 插件

1. 下载 [filterblade-zh-extension.zip](https://cdn.jsdelivr.net/gh/ExileKwin/filterblade-zh@main/filterblade-zh-extension.zip) 并解压到一个固定目录（解压后不要删除）
2. 浏览器地址栏打开 `chrome://extensions`
3. 右上角打开 **开发者模式**
4. 点 **加载已解压的扩展程序**，选中刚才解压出来的文件夹
5. 打开 filterblade，左下角出现「中文补全」面板即成功

Edge 同理，地址是 `edge://extensions`。

## 使用

安装后无需配置，页面自动中文化。左下角面板有三个功能：

- **采集**：把页面上尚未翻译的英文导出成 CSV
- **导入**：载入词典文件（JSON 或 CSV）
- **重新应用**：页面文案被网站重新渲染时可手动再翻一次

## 词典与译名来源

内置词典共 **9512 条**，覆盖导航栏、筛选项、区块标题、物品基底、通货、词缀、音效与颜色面板。

**译名来源分三层：**

| 范围 | 依据 |
|---|---|
| 物品基底、通货、化石、圣油、催化剂、词缀 | 参照 [poedb.tw](https://poedb.tw/cn/) 的国服官方译名逐条校对 |
| 界面用语、说明文案、区块标题 | 采用 PoE 中文社区长期通用的译法 |
| 筛选器语法（`SetFontSize`、`Class ==` 等） | 保留原文，翻译会改变过滤器语义 |

**完成度：** 以站内实际采集结果为基准，界面可见文本已全部汉化。最近一次整站采集共 1103 条未翻译文本，已全部补齐，采集复扫无残留。

页面上的英文只剩两类「本就应该保留」的内容：筛选器代码字面量，以及掉落模拟器随机生成的物品组合。

## 作者

Kwin

## 更新

版本号跟随游戏赛季，例如 `3.30` 对应 3.30 赛季。新赛季有新物品时，词典会同步补充并升级版本号。

用户脚本版本内置了更新地址，Tampermonkey 会自动检测新版本；插件版本需重新下载压缩包并按上面步骤覆盖加载。

## 许可

MIT
