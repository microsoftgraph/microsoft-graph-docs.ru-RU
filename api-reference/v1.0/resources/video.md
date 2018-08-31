---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Video
ms.openlocfilehash: cb9e28c1b26aa60fe7d854796df8bff34ca8e5df
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265850"
---
# <a name="video-resource-type"></a><span data-ttu-id="da4ca-102">Тип ресурса video</span><span class="sxs-lookup"><span data-stu-id="da4ca-102">Video resource type</span></span>

<span data-ttu-id="da4ca-103">Ресурс **Video** — это единая структура, объединяющая элементы данных, связанные с видео.</span><span class="sxs-lookup"><span data-stu-id="da4ca-103">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="da4ca-p101">Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **video**, то этот ресурс представляет видеофайл. Свойства ресурса **Video** заполняются путем извлечения метаданных из такого файла.</span><span class="sxs-lookup"><span data-stu-id="da4ca-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="da4ca-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da4ca-106">JSON representation</span></span>

<span data-ttu-id="da4ca-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="da4ca-107">Here is a JSON representation of the resource</span></span>

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
  "frameRate": 239.877,
  "height": 1280,
  "width": 720
}
```

## <a name="properties"></a><span data-ttu-id="da4ca-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="da4ca-108">Properties</span></span>

| <span data-ttu-id="da4ca-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="da4ca-109">Property name</span></span>             | <span data-ttu-id="da4ca-110">Тип</span><span class="sxs-lookup"><span data-stu-id="da4ca-110">Type</span></span>   | <span data-ttu-id="da4ca-111">Описание</span><span class="sxs-lookup"><span data-stu-id="da4ca-111">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="da4ca-112">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="da4ca-112">**audioBitsPerSample**</span></span>    | <span data-ttu-id="da4ca-113">Int32</span><span class="sxs-lookup"><span data-stu-id="da4ca-113">Int32</span></span>  | <span data-ttu-id="da4ca-114">Количество разрядов звука на выборку.</span><span class="sxs-lookup"><span data-stu-id="da4ca-114">Number of audio bits per sample.</span></span>
| <span data-ttu-id="da4ca-115">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="da4ca-115">**audioChannels**</span></span>         | <span data-ttu-id="da4ca-116">Int32</span><span class="sxs-lookup"><span data-stu-id="da4ca-116">Int32</span></span>  | <span data-ttu-id="da4ca-117">Количество звуковых каналов.</span><span class="sxs-lookup"><span data-stu-id="da4ca-117">Number of audio channels.</span></span>
| <span data-ttu-id="da4ca-118">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="da4ca-118">**audioFormat**</span></span>           | <span data-ttu-id="da4ca-119">строка</span><span class="sxs-lookup"><span data-stu-id="da4ca-119">string</span></span> | <span data-ttu-id="da4ca-120">Название формата аудио (AAC, MP3, и т. д.).</span><span class="sxs-lookup"><span data-stu-id="da4ca-120">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="da4ca-121">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="da4ca-121">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="da4ca-122">Int32</span><span class="sxs-lookup"><span data-stu-id="da4ca-122">Int32</span></span>  | <span data-ttu-id="da4ca-123">Количество выборок звука в секунду.</span><span class="sxs-lookup"><span data-stu-id="da4ca-123">Number of audio samples per second.</span></span>
| <span data-ttu-id="da4ca-124">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="da4ca-124">**bitrate**</span></span>               | <span data-ttu-id="da4ca-125">Int32</span><span class="sxs-lookup"><span data-stu-id="da4ca-125">Int32</span></span>  | <span data-ttu-id="da4ca-126">Скорость видео в битах в секунду.</span><span class="sxs-lookup"><span data-stu-id="da4ca-126">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="da4ca-127">**duration**</span><span class="sxs-lookup"><span data-stu-id="da4ca-127">**duration**</span></span>              | <span data-ttu-id="da4ca-128">Int64</span><span class="sxs-lookup"><span data-stu-id="da4ca-128">Int64</span></span>  | <span data-ttu-id="da4ca-129">Длительность файла в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="da4ca-129">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="da4ca-130">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="da4ca-130">**fourCC**</span></span>                | <span data-ttu-id="da4ca-131">строка</span><span class="sxs-lookup"><span data-stu-id="da4ca-131">string</span></span> | <span data-ttu-id="da4ca-132">Название формата видео в виде четырехзначного кода.</span><span class="sxs-lookup"><span data-stu-id="da4ca-132">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="da4ca-133">**frameRate**</span><span class="sxs-lookup"><span data-stu-id="da4ca-133">**framerate**</span></span>             | <span data-ttu-id="da4ca-134">double</span><span class="sxs-lookup"><span data-stu-id="da4ca-134">double</span></span> | <span data-ttu-id="da4ca-135">Частота кадров видео.</span><span class="sxs-lookup"><span data-stu-id="da4ca-135">Frame rate of the video.</span></span>
| <span data-ttu-id="da4ca-136">**height**</span><span class="sxs-lookup"><span data-stu-id="da4ca-136">**height**</span></span>                | <span data-ttu-id="da4ca-137">Int32</span><span class="sxs-lookup"><span data-stu-id="da4ca-137">Int32</span></span>  | <span data-ttu-id="da4ca-138">Высота видео в пикселях.</span><span class="sxs-lookup"><span data-stu-id="da4ca-138">Height of the video, in pixels.</span></span>
| <span data-ttu-id="da4ca-139">**width**</span><span class="sxs-lookup"><span data-stu-id="da4ca-139">**width**</span></span>                 | <span data-ttu-id="da4ca-140">Int32</span><span class="sxs-lookup"><span data-stu-id="da4ca-140">Int32</span></span>  | <span data-ttu-id="da4ca-141">Ширина видео в пикселях.</span><span class="sxs-lookup"><span data-stu-id="da4ca-141">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="da4ca-142">Замечания</span><span class="sxs-lookup"><span data-stu-id="da4ca-142">Remarks</span></span>

<span data-ttu-id="da4ca-143">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="da4ca-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->
