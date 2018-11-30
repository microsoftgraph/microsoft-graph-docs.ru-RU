---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Video
ms.openlocfilehash: a9bf228d814526d089fb102444e6952558b07e1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081609"
---
# <a name="video-resource-type"></a><span data-ttu-id="7b5ff-102">Тип ресурса video</span><span class="sxs-lookup"><span data-stu-id="7b5ff-102">Video resource type</span></span>

> <span data-ttu-id="7b5ff-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7b5ff-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b5ff-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b5ff-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b5ff-105">Ресурс **Video** — это единая структура, объединяющая элементы данных, связанные с видео.</span><span class="sxs-lookup"><span data-stu-id="7b5ff-105">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="7b5ff-p102">Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **video**, то этот ресурс представляет видеофайл. Свойства ресурса **Video** заполняются путем извлечения метаданных из такого файла.</span><span class="sxs-lookup"><span data-stu-id="7b5ff-p102">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b5ff-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b5ff-108">JSON representation</span></span>

<span data-ttu-id="7b5ff-109">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="7b5ff-109">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="7b5ff-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b5ff-110">Properties</span></span>

| <span data-ttu-id="7b5ff-111">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7b5ff-111">Property name</span></span>             | <span data-ttu-id="7b5ff-112">Тип</span><span class="sxs-lookup"><span data-stu-id="7b5ff-112">Type</span></span>   | <span data-ttu-id="7b5ff-113">Описание</span><span class="sxs-lookup"><span data-stu-id="7b5ff-113">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="7b5ff-114">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="7b5ff-114">**audioBitsPerSample**</span></span>    | <span data-ttu-id="7b5ff-115">Int32</span><span class="sxs-lookup"><span data-stu-id="7b5ff-115">Int32</span></span>  | <span data-ttu-id="7b5ff-116">Количество разрядов звука на выборку.</span><span class="sxs-lookup"><span data-stu-id="7b5ff-116">Number of audio bits per sample.</span></span>
| <span data-ttu-id="7b5ff-117">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="7b5ff-117">**audioChannels**</span></span>         | <span data-ttu-id="7b5ff-118">Int32</span><span class="sxs-lookup"><span data-stu-id="7b5ff-118">Int32</span></span>  | <span data-ttu-id="7b5ff-119">Количество звуковых каналов.</span><span class="sxs-lookup"><span data-stu-id="7b5ff-119">Number of audio channels.</span></span>
| <span data-ttu-id="7b5ff-120">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="7b5ff-120">**audioFormat**</span></span>           | <span data-ttu-id="7b5ff-121">строка</span><span class="sxs-lookup"><span data-stu-id="7b5ff-121">string</span></span> | <span data-ttu-id="7b5ff-122">Название формата аудио (AAC, MP3, и т. д.).</span><span class="sxs-lookup"><span data-stu-id="7b5ff-122">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="7b5ff-123">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="7b5ff-123">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="7b5ff-124">Int32</span><span class="sxs-lookup"><span data-stu-id="7b5ff-124">Int32</span></span>  | <span data-ttu-id="7b5ff-125">Количество выборок звука в секунду.</span><span class="sxs-lookup"><span data-stu-id="7b5ff-125">Number of audio samples per second.</span></span>
| <span data-ttu-id="7b5ff-126">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="7b5ff-126">**bitrate**</span></span>               | <span data-ttu-id="7b5ff-127">Int32</span><span class="sxs-lookup"><span data-stu-id="7b5ff-127">Int32</span></span>  | <span data-ttu-id="7b5ff-128">Скорость видео в битах в секунду.</span><span class="sxs-lookup"><span data-stu-id="7b5ff-128">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="7b5ff-129">**duration**</span><span class="sxs-lookup"><span data-stu-id="7b5ff-129">**duration**</span></span>              | <span data-ttu-id="7b5ff-130">Int64</span><span class="sxs-lookup"><span data-stu-id="7b5ff-130">Int64</span></span>  | <span data-ttu-id="7b5ff-131">Длительность файла в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="7b5ff-131">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="7b5ff-132">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="7b5ff-132">**fourCC**</span></span>                | <span data-ttu-id="7b5ff-133">строка</span><span class="sxs-lookup"><span data-stu-id="7b5ff-133">string</span></span> | <span data-ttu-id="7b5ff-134">Название формата видео в виде четырехзначного кода.</span><span class="sxs-lookup"><span data-stu-id="7b5ff-134">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="7b5ff-135">**framerate**</span><span class="sxs-lookup"><span data-stu-id="7b5ff-135">**framerate**</span></span>             | <span data-ttu-id="7b5ff-136">double</span><span class="sxs-lookup"><span data-stu-id="7b5ff-136">double</span></span> | <span data-ttu-id="7b5ff-137">Частота кадров видео.</span><span class="sxs-lookup"><span data-stu-id="7b5ff-137">Frame rate of the video.</span></span>
| <span data-ttu-id="7b5ff-138">**height**</span><span class="sxs-lookup"><span data-stu-id="7b5ff-138">**height**</span></span>                | <span data-ttu-id="7b5ff-139">Int32</span><span class="sxs-lookup"><span data-stu-id="7b5ff-139">Int32</span></span>  | <span data-ttu-id="7b5ff-140">Высота видео в пикселях.</span><span class="sxs-lookup"><span data-stu-id="7b5ff-140">Height of the video, in pixels.</span></span>
| <span data-ttu-id="7b5ff-141">**width**</span><span class="sxs-lookup"><span data-stu-id="7b5ff-141">**width**</span></span>                 | <span data-ttu-id="7b5ff-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7b5ff-142">Int32</span></span>  | <span data-ttu-id="7b5ff-143">Ширина видео в пикселях.</span><span class="sxs-lookup"><span data-stu-id="7b5ff-143">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="7b5ff-144">Замечания</span><span class="sxs-lookup"><span data-stu-id="7b5ff-144">Remarks</span></span>

<span data-ttu-id="7b5ff-145">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="7b5ff-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": ""
}-->
