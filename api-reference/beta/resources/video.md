---
author: JeremyKelley
description: Ресурс Video — это единая структура, объединяющая элементы данных, связанные с видео.
ms.date: 09/10/2017
title: Видео
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b80d36ce35a950fa20424124b20cba34c19307c3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519472"
---
# <a name="video-resource-type"></a><span data-ttu-id="4514a-103">Тип ресурса video</span><span class="sxs-lookup"><span data-stu-id="4514a-103">Video resource type</span></span>

<span data-ttu-id="4514a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4514a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4514a-105">Ресурс **Video** — это единая структура, объединяющая элементы данных, связанные с видео.</span><span class="sxs-lookup"><span data-stu-id="4514a-105">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="4514a-p101">Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **video**, то этот ресурс представляет видеофайл. Свойства ресурса **Video** заполняются путем извлечения метаданных из такого файла.</span><span class="sxs-lookup"><span data-stu-id="4514a-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4514a-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4514a-108">JSON representation</span></span>

<span data-ttu-id="4514a-109">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="4514a-109">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.video"
}-->

```json
{
  "audioBitsPerSample": 16,
  "audioChannels": 1,
  "audioFormat": "AAC",
  "audioSamplesPerSecond": 44100,
  "bitrate": 39101896,
  "duration": 8053,
  "fourCC": "H264",
  "height": 1280,
  "width": 720,
  "framerate": 2.75
}
```

## <a name="properties"></a><span data-ttu-id="4514a-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="4514a-110">Properties</span></span>

| <span data-ttu-id="4514a-111">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="4514a-111">Property name</span></span>             | <span data-ttu-id="4514a-112">Тип</span><span class="sxs-lookup"><span data-stu-id="4514a-112">Type</span></span>   | <span data-ttu-id="4514a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="4514a-113">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="4514a-114">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="4514a-114">**audioBitsPerSample**</span></span>    | <span data-ttu-id="4514a-115">Int32</span><span class="sxs-lookup"><span data-stu-id="4514a-115">Int32</span></span>  | <span data-ttu-id="4514a-116">Количество разрядов звука на выборку.</span><span class="sxs-lookup"><span data-stu-id="4514a-116">Number of audio bits per sample.</span></span>
| <span data-ttu-id="4514a-117">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="4514a-117">**audioChannels**</span></span>         | <span data-ttu-id="4514a-118">Int32</span><span class="sxs-lookup"><span data-stu-id="4514a-118">Int32</span></span>  | <span data-ttu-id="4514a-119">Количество звуковых каналов.</span><span class="sxs-lookup"><span data-stu-id="4514a-119">Number of audio channels.</span></span>
| <span data-ttu-id="4514a-120">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="4514a-120">**audioFormat**</span></span>           | <span data-ttu-id="4514a-121">string</span><span class="sxs-lookup"><span data-stu-id="4514a-121">string</span></span> | <span data-ttu-id="4514a-122">Название формата аудио (AAC, MP3, и т. д.).</span><span class="sxs-lookup"><span data-stu-id="4514a-122">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="4514a-123">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="4514a-123">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="4514a-124">Int32</span><span class="sxs-lookup"><span data-stu-id="4514a-124">Int32</span></span>  | <span data-ttu-id="4514a-125">Количество выборок звука в секунду.</span><span class="sxs-lookup"><span data-stu-id="4514a-125">Number of audio samples per second.</span></span>
| <span data-ttu-id="4514a-126">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="4514a-126">**bitrate**</span></span>               | <span data-ttu-id="4514a-127">Int32</span><span class="sxs-lookup"><span data-stu-id="4514a-127">Int32</span></span>  | <span data-ttu-id="4514a-128">Скорость видео в битах в секунду.</span><span class="sxs-lookup"><span data-stu-id="4514a-128">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="4514a-129">**duration**</span><span class="sxs-lookup"><span data-stu-id="4514a-129">**duration**</span></span>              | <span data-ttu-id="4514a-130">Int64</span><span class="sxs-lookup"><span data-stu-id="4514a-130">Int64</span></span>  | <span data-ttu-id="4514a-131">Длительность файла в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="4514a-131">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="4514a-132">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="4514a-132">**fourCC**</span></span>                | <span data-ttu-id="4514a-133">string</span><span class="sxs-lookup"><span data-stu-id="4514a-133">string</span></span> | <span data-ttu-id="4514a-134">Название формата видео в виде четырехзначного кода.</span><span class="sxs-lookup"><span data-stu-id="4514a-134">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="4514a-135">**framerate**</span><span class="sxs-lookup"><span data-stu-id="4514a-135">**framerate**</span></span>             | <span data-ttu-id="4514a-136">double</span><span class="sxs-lookup"><span data-stu-id="4514a-136">double</span></span> | <span data-ttu-id="4514a-137">Частота кадров видео.</span><span class="sxs-lookup"><span data-stu-id="4514a-137">Frame rate of the video.</span></span>
| <span data-ttu-id="4514a-138">**height**</span><span class="sxs-lookup"><span data-stu-id="4514a-138">**height**</span></span>                | <span data-ttu-id="4514a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4514a-139">Int32</span></span>  | <span data-ttu-id="4514a-140">Высота видео в пикселях.</span><span class="sxs-lookup"><span data-stu-id="4514a-140">Height of the video, in pixels.</span></span>
| <span data-ttu-id="4514a-141">**width**</span><span class="sxs-lookup"><span data-stu-id="4514a-141">**width**</span></span>                 | <span data-ttu-id="4514a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4514a-142">Int32</span></span>  | <span data-ttu-id="4514a-143">Ширина видео в пикселях.</span><span class="sxs-lookup"><span data-stu-id="4514a-143">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="4514a-144">Заметки</span><span class="sxs-lookup"><span data-stu-id="4514a-144">Remarks</span></span>

<span data-ttu-id="4514a-145">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="4514a-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
