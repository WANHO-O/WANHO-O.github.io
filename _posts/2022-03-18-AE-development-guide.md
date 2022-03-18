---
layout: article
title: AE plug-ins SampleProjects guide
mathjax: true
---

# AEGPs

AEGP 直接连接到 After Effects 的菜单和 UI 中的其他区域。有关 AEGP 在 UI 中显示位置的详细信息，请参见下文。

## Artie

Artie the Artisan 接管了给定合成中所有 3D 图层的渲染。这与我们内部 3D 渲染器使用的 API 相同；它非常复杂，并且暴露了大量关于 After Effects 渲染管道
的隐性信息。除非您有令人信服的理由来替换 After Effects 处理 3D 渲染的方式，否则您永远不需要使用此示例。Artisans 出现在“合成”>“合成设置”的“高级”选项
卡的“渲染插件”下拉菜单中。

## Easy Cheese

关键帧生成器（显示在“动画”>“关键帧助手”子菜单中），Easy Cheese 展示了如何操纵关键帧的各种特征（以一种不可思议的方式，类似于我们的发货插件，Easy Ease……）

## FBIO

练习 After Effects 输入/输出 (AEIO) API。类似于 IO 示例，但支持基于帧的 .ffk 文件格式。请注意，我们现在建议改为开发 Premiere Pro Importers 。

## Grabba

从项目中的任何合成中获取帧（格式化为插件请求）。

## IO

练习 After Effects 输入/输出 (AEIO) API。支持虚构.fak 文件格式，并处理来自 After Effects 的所有请求，以从此类文件中检索数据或输出到此类文件。请注
意，我们现在建议改为开发 Premiere Pro Importers 。

## Mangler

Mangler 是一个关键帧生成器，演示了 ADM 调色板的使用，就像我们自己的一样。

## Panelator

创建一个可以与其他标准面板一起停靠的面板。注意：以这种方式创建面板比使用 HTML5 面板 SDK 要做的工作要多得多。我们建议从该 SDK 开始。

## Persisto

显示如何从 After Effects 首选项文件中读取和写入信息。

## ProjDumper

创建一个表示 After Effects 项目中每个元素的文本文件。

## Projector

导入（虚构的）.sdk 文件格式，并使用 AEGP API 调用创建项目。每当您想知道如何获取或设置项目元素的某些特征时，请先查看此处。注意：Projector.h 中有一些硬编
码路径。如果您不将这些设置为引用磁盘上的实际媒体，则在运行此插件时会出错。不要怪我们；改变他们！

## QueueBert

发音为“Cue-BARE！”，QueueBert 操作渲染队列项目的所有方面以及与它们相关的输出模块。

## Streamie

处理动态和固定的流。

## Sweetie

Sweetie 使用 PICA（或“Suite Pea”）API 来提供一个功能套件，供其他插件使用。如果您正在编写依赖于同一个图像处理库的多个插件，您可以使用这样的套件来提供库功
能。

## Text Twiddler

操作文本层及其内容。

## Effects

所有效果都出现在“效果与预设”面板和“效果”菜单中。

## Checkout

在指定时间检出（从 After Effects 的帧缓存中）来自另一层的输入帧。对于所有具有图层参数的效果，这是一个重要的概念。兼容 Premiere Pro。

## Convolutrix

练习我们的图像卷积回调。兼容 Premiere Pro。

## Gamma Table

展示如何管理序列数据，并使用我们的迭代回调。为了怀旧，我们将这个样本留在 C 中；由于它依赖于版本 3.x API 功能，它还与许多第三方插件主机兼容。

## GLator

CC 2017 的新功能。在效果插件中演示正确的 OpenGL 上下文管理。

## Paramarama

习其他示例中未使用的任意参数类型。兼容 Premiere Pro。

## PathMaster

显示如何从效果中访问路径。

## Portable

展示如何检测和响应几个不同的插件主机。兼容 Premiere Pro。

## Resizer

Resizer 调整输出缓冲区的大小（惊喜！）。这对于像发光和阴影这样的效果很有用，如果它们没有扩展输出缓冲区，它们会在图层边缘被截断。兼容 Premiere Pro。

## SDK Backwards

反转图层的音频，并将其与可关键帧的正弦波混合。

## SDK Noise

Premiere Pro 兼容，在 Premiere Pro 中演示 32 位和 YUV 渲染。

## Shifter

移动输出缓冲区中的图像，并练习我们的 transform_world 和亚像素采样函数。

## SmartyPants

演示支持浮点像素所需的 SmartFX API。

## Transformer

练习我们的图像转换回调。

# Effect Template

## Skeleton

骨架是开发效果的起点。兼容 Premiere Pro。

# Effects with Custom UI

## CCU

在合成和图层窗口中实现自定义用户界面，支持像素纵横比和下采样率。兼容 Premiere Pro。

## ColorGrid

显示如何使用任意数据类型参数。也有一个很好的自定义用户界面。兼容 Premiere Pro。

## Custom ECW UI

在效果控件窗口中实现了一个非常无聊的自定义用户界面，并展示了如何响应众多 UI 事件。

## Histogrid

CC 2015 (13.5) 的新功能。自定义 UI 如何访问异步渲染的上游帧以在 CC 2015 及更高版本中进行轻量级处理的示例。此效果从上游帧计算采样的 10x10 颜色网格，
并显示该颜色网格的预览。在渲染中，更高质量的网格被计算并用于修改输出图像，创建颜色网格与原始图像的混合。

## Supervisor

显示如何根据其他参数的值控制参数（值和 UI）。兼容 Premiere Pro。

# BlitHook

## EMP

外部监视器预览。以此为起点，添加对从合成面板输出视频到视频硬件的支持。
