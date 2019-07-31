---
author: JeremyKelley
description: Ресурс Video — это единая структура, объединяющая элементы данных, связанные с видео.
ms.date: 09/10/2017
title: Видео
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e93fd4bbd348df3ad31d1be6aa2b1dc73593327a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007363"
---
# <a name="video-resource-type"></a><span data-ttu-id="d650a-103">Тип ресурса video</span><span class="sxs-lookup"><span data-stu-id="d650a-103">Video resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d650a-104">Ресурс **Video** — это единая структура, объединяющая элементы данных, связанные с видео.</span><span class="sxs-lookup"><span data-stu-id="d650a-104">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="d650a-p101">Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **video**, то этот ресурс представляет видеофайл. Свойства ресурса **Video** заполняются путем извлечения метаданных из такого файла.</span><span class="sxs-lookup"><span data-stu-id="d650a-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d650a-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d650a-107">JSON representation</span></span>

<span data-ttu-id="d650a-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="d650a-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="d650a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d650a-109">Properties</span></span>

| <span data-ttu-id="d650a-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="d650a-110">Property name</span></span>             | <span data-ttu-id="d650a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d650a-111">Type</span></span>   | <span data-ttu-id="d650a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d650a-112">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="d650a-113">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="d650a-113">**audioBitsPerSample**</span></span>    | <span data-ttu-id="d650a-114">Int32</span><span class="sxs-lookup"><span data-stu-id="d650a-114">Int32</span></span>  | <span data-ttu-id="d650a-115">Количество разрядов звука на выборку.</span><span class="sxs-lookup"><span data-stu-id="d650a-115">Number of audio bits per sample.</span></span>
| <span data-ttu-id="d650a-116">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="d650a-116">**audioChannels**</span></span>         | <span data-ttu-id="d650a-117">Int32</span><span class="sxs-lookup"><span data-stu-id="d650a-117">Int32</span></span>  | <span data-ttu-id="d650a-118">Количество звуковых каналов.</span><span class="sxs-lookup"><span data-stu-id="d650a-118">Number of audio channels.</span></span>
| <span data-ttu-id="d650a-119">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="d650a-119">**audioFormat**</span></span>           | <span data-ttu-id="d650a-120">string</span><span class="sxs-lookup"><span data-stu-id="d650a-120">string</span></span> | <span data-ttu-id="d650a-121">Название формата аудио (AAC, MP3, и т. д.).</span><span class="sxs-lookup"><span data-stu-id="d650a-121">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="d650a-122">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="d650a-122">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="d650a-123">Int32</span><span class="sxs-lookup"><span data-stu-id="d650a-123">Int32</span></span>  | <span data-ttu-id="d650a-124">Количество выборок звука в секунду.</span><span class="sxs-lookup"><span data-stu-id="d650a-124">Number of audio samples per second.</span></span>
| <span data-ttu-id="d650a-125">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="d650a-125">**bitrate**</span></span>               | <span data-ttu-id="d650a-126">Int32</span><span class="sxs-lookup"><span data-stu-id="d650a-126">Int32</span></span>  | <span data-ttu-id="d650a-127">Скорость видео в битах в секунду.</span><span class="sxs-lookup"><span data-stu-id="d650a-127">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="d650a-128">**duration**</span><span class="sxs-lookup"><span data-stu-id="d650a-128">**duration**</span></span>              | <span data-ttu-id="d650a-129">Int64</span><span class="sxs-lookup"><span data-stu-id="d650a-129">Int64</span></span>  | <span data-ttu-id="d650a-130">Длительность файла в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="d650a-130">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="d650a-131">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="d650a-131">**fourCC**</span></span>                | <span data-ttu-id="d650a-132">string</span><span class="sxs-lookup"><span data-stu-id="d650a-132">string</span></span> | <span data-ttu-id="d650a-133">Название формата видео в виде четырехзначного кода.</span><span class="sxs-lookup"><span data-stu-id="d650a-133">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="d650a-134">**framerate**</span><span class="sxs-lookup"><span data-stu-id="d650a-134">**framerate**</span></span>             | <span data-ttu-id="d650a-135">double</span><span class="sxs-lookup"><span data-stu-id="d650a-135">double</span></span> | <span data-ttu-id="d650a-136">Частота кадров видео.</span><span class="sxs-lookup"><span data-stu-id="d650a-136">Frame rate of the video.</span></span>
| <span data-ttu-id="d650a-137">**height**</span><span class="sxs-lookup"><span data-stu-id="d650a-137">**height**</span></span>                | <span data-ttu-id="d650a-138">Int32</span><span class="sxs-lookup"><span data-stu-id="d650a-138">Int32</span></span>  | <span data-ttu-id="d650a-139">Высота видео в пикселях.</span><span class="sxs-lookup"><span data-stu-id="d650a-139">Height of the video, in pixels.</span></span>
| <span data-ttu-id="d650a-140">**width**</span><span class="sxs-lookup"><span data-stu-id="d650a-140">**width**</span></span>                 | <span data-ttu-id="d650a-141">Int32</span><span class="sxs-lookup"><span data-stu-id="d650a-141">Int32</span></span>  | <span data-ttu-id="d650a-142">Ширина видео в пикселях.</span><span class="sxs-lookup"><span data-stu-id="d650a-142">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="d650a-143">Заметки</span><span class="sxs-lookup"><span data-stu-id="d650a-143">Remarks</span></span>

<span data-ttu-id="d650a-144">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="d650a-144">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>





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
