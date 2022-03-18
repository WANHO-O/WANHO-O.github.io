---
layout: article
title: AE plug-ing-AEGP-DataType-guide
mathjax: true
---

> ## AEGP_MemHandle --- [AEGP Memory Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-memory-suite)
>
> 这个结构不仅仅包含引用的内存。所以不应该直接取消引用。AEGP_LockMemHandle 在 AEGP 内存套件中使用以获取指向 AEGP_MemHandle. 当然，完成后解锁它。

> ## AEGP_ProjectH --- [AEGP Project Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-project-suite)
>
> 当前的 After Effects 项目。项目是在树中分层排列的一组元素，以保留语义关系。树的内部节点是文件夹。从 CS6 开始，只会有一个打开的项目。

> ## AEGP_ItemH --- [AEGP Item Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-item-suite)
>
> 描述项目的任何元素的抽象，包括文件夹。项目是可以选择的任何东西。由于可以选择多个对象类型，我们将它们视为 AEGP_ItemHs，直到需要更多特异性。

> ## AEGP_Collection2H --- [AEGP Collection Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-item-suite)
>
> 一组选定的项目。

> ## AEGP_Comp --- [AEGP Composition Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-composition-suite)
>
> 组合是一系列可渲染项目，它们一起产生输出。一个组合存在于一个时间间隔内。一个项目中可以存在多个组合。

> ## AEGP_FootageH --- [AEGP Footage Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-footage-suite)
>
> 可以渲染的项目。文件夹和作品是唯一不是素材的项目。

> ## AEGP_LayerH --- [AEGP Layer Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-layer-suite)
>
> 组合的一个元素。图层按顺序渲染，允许遮挡。实体、文本、油漆、相机、灯光、图像和图像序列都表示为层。可以在组合的时间间隔的子间隔上定义层。

> ## AEGP_WorldH ---[AEGP World Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-world-suite)
>
> 一帧像素。

> ## AEGP_EffectRefH --- [AEGP Effect Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-effect-suite)
>
> 应用于图层的效果。效果是一个函数，它以图层（可能还有其他参数）为参数，并返回图层的更改版本以进行渲染。

> ## AEGP_StreamRefH --- [AEGP Stream Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-stream-suite), [AEGP Dynamic Stream Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-dynamic-stream-suite), [AEGP Keyframe Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-keyframe-suite)
>
> 在合成中附加到图层的任何参数流。有关流类型的完整列表，请参阅 AEGP_GetNewLayerStream 来自 AEGP_StreamSuite5 的描述。

> ## AEGP_MaskRefH --- [AEGP Mask Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-mask-suite)
>
> 应用于图层的蒙版。AEGP_MaskRefH 用于访问有关掩码流的详细信息，而不是构成掩码的特定点。蒙版是一个光栅化路径（顶点序列），它将一个层分成两部分，允许以不同的方式渲染每一部分。

> ## AEGP_MaskOutlineValH --- [AEGP Mask Outline Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-mask-outline-suite)
>
> 构成掩码的具体点。掩码轮廓中的点是有序的，掩码不需要关闭。

> ## AEGP_TextDocumentH --- [AEGP Text Document Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-text-document-suite)
>
> 表示与文本图层关联的实际文本。

> ## AEGP_TextOutlinesH --- [AEGP Text Layer Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-text-layer-suite)
>
> 构成给定文本层轮廓的所有路径的引用。

> ## AEGP_MarkerVal --- [AEGP Marker Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-marker-suite)
>
> 与给定时间线标记关联的数据。

> ## AEGP_PersistentBlobH --- [AEGP Persistent Data Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-persistent-data-suite)
>
> 包含当前偏好的数据“块”。

> ## AEGP_RenderOptionsH --- [AEGP Render Options Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-render-options-suite)
>
> 与呈现请求关联的设置。

> ## AEGP_LayerRenderOptionsH --- [AEGP Layer Render Options Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-aegp-layerrenderoptionssuite)
>
> 与图层渲染请求关联的设置。

> ## AEGP_FrameReceiptH --- [AEGP Render Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-render-suite)
>
> 对渲染帧的引用。

> ## AEGP_RQItemRefH --- [AEGP Render Queue Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-render-queue-suite) ,[AEGP Render Queue Item Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-render-queue-item-suite)
>
> 渲染队列中的一个项目。

> ## AEGP_OutputModuleRefH --- [AEGP Output Module Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-output-module-suite)
>
> 一个输出模块，附加到渲染队列中的特定 AEGP_RQItemRef。

> ## AEGP_SoundDataH --- [AEGP Sound Data Suite](https://ae-plugins.docsforadobe.dev/aegps/aegp-suites.html#aegps-aegp-suites-sound-data-suite)
>
> 用于给定层的音频设置。

> ## AEGP_RenderLayerContextH --- [AEGP Canvas Suite](https://ae-plugins.docsforadobe.dev/artisans/artisan-data-types.html#artisans-artisan-data-types-aegp-canvassuite)
>
> 渲染请求时的状态信息，由 After Effects 发送给 Artisan。

> ## AEGP_RenderReceiptH --- [AEGP Canvas Suite](https://ae-plugins.docsforadobe.dev/artisans/artisan-data-types.html#artisans-artisan-data-types-aegp-canvassuite)
>
> 由工匠在渲染时使用。
