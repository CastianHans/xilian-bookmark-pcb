# 昔涟如我所书 · 沉金书签 PCB

一个 56 × 99 mm 的艺术 PCB 书签工程，面向嘉立创 EDA / PCB 打样。

## 先看这里：正确下载包

- [正确包：ENIG 沉金描边 + 彩色丝印（推荐上传）](production/xilian-bookmark-pcb-ENIG-color-upload-ready.zip)
- [嘉立创 EDA 专业版工程（EPRO，推荐打开）](easyeda/ProPrj_Bookmark_Art_PCB_56x99_ENIG_Vector_final_2026-09-28.epro)
- [兼容旧链接的同一正确包](production/bookmark-pcb-jlc-upload-ready.zip)
- [完整矢量与制造文件](artwork/)
- [生产预览图](preview/)

不要下载或上传 `archive/not-for-production/` 中的文件。那里面是此前的空工程/原始留档，只用于追溯问题，里面的 `GTL/GTS` 没有沉金描边。

## 当前规格

- 外形：56.00 × 99.00 mm，圆角 R3.00 mm
- 板材：2 层 FR-4
- 板厚：1.6 mm
- 阻焊：白色
- 表面处理：沉金（ENIG）
- 正面：彩色丝印 + 描边沉金
- 背面：当前下单版本为空白白色阻焊面
- 钻孔：无
- 拼板：不拼板，单片出货

## 文件说明

```text
artwork/                  矢量彩色丝印、沉金线稿、板框
easyeda/                  嘉立创 EDA 专业版工程与导出留档
production/               可直接用于生产的下单包及展开文件
preview/                  金属层和整板预览，仅用于核对
docs/                     制造清单、规格和 SHA-256 清单
archive/                  明确标记为不可生产的历史留档
```

生产时只使用 `production/xilian-bookmark-pcb-ENIG-color-upload-ready.zip`（或兼容旧链接的同一正确包）。不要把预览 PNG 当作 Gerber 上传，也不要单独替换 ZIP 内同名的彩色丝印、铜层或阻焊层文件。

正确包内必须同时存在并且有内容：`Gerber_TopLayer.GTL`（沉金铜线）和 `Gerber_TopSolderMaskLayer.GTS`（沉金开窗）。

## 制造提醒

这是艺术 PCB 文件，不是带电路功能的电子产品。下单前请在嘉立创 CAM 预览中重新核对板框尺寸、正反面方向、彩色丝印位置和沉金开窗；任何平台自动修复或坐标偏移都应先人工确认。

本仓库公开的是工程和生产资料。原始角色/插画元素的著作权不由本仓库作者主张；请勿将原图或由其产生的商品用于未经授权的商业用途。

## 校验

完整文件清单和 SHA-256 校验值见 [`docs/manifest.json`](docs/manifest.json)。历史问题说明见 [`archive/not-for-production/README.md`](archive/not-for-production/README.md)。
