---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Video
localization_priority: Normal
ms.openlocfilehash: db560abc31daecc6064820ef6ef958808ddbc297
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508547"
---
# <a name="video-resource-type"></a><span data-ttu-id="257df-102">Тип ресурса video</span><span class="sxs-lookup"><span data-stu-id="257df-102">Video resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="257df-103">Ресурс **Video** — это единая структура, объединяющая элементы данных, связанные с видео.</span><span class="sxs-lookup"><span data-stu-id="257df-103">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="257df-p101">Если у ресурса DriveItem есть ненулевой аспект video, то этот ресурс представляет видеофайл. Свойства ресурса Video заполняются путем извлечения метаданных из такого файла.</span><span class="sxs-lookup"><span data-stu-id="257df-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="257df-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="257df-106">JSON representation</span></span>

<span data-ttu-id="257df-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="257df-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="257df-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="257df-108">Properties</span></span>

| <span data-ttu-id="257df-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="257df-109">Property name</span></span>             | <span data-ttu-id="257df-110">Тип</span><span class="sxs-lookup"><span data-stu-id="257df-110">Type</span></span>   | <span data-ttu-id="257df-111">Описание</span><span class="sxs-lookup"><span data-stu-id="257df-111">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="257df-112">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="257df-112">**audioBitsPerSample**</span></span>    | <span data-ttu-id="257df-113">Int32</span><span class="sxs-lookup"><span data-stu-id="257df-113">Int32</span></span>  | <span data-ttu-id="257df-114">Количество разрядов звука на выборку.</span><span class="sxs-lookup"><span data-stu-id="257df-114">Number of audio bits per sample.</span></span>
| <span data-ttu-id="257df-115">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="257df-115">**audioChannels**</span></span>         | <span data-ttu-id="257df-116">Int32</span><span class="sxs-lookup"><span data-stu-id="257df-116">Int32</span></span>  | <span data-ttu-id="257df-117">Количество звуковых каналов.</span><span class="sxs-lookup"><span data-stu-id="257df-117">Number of audio channels.</span></span>
| <span data-ttu-id="257df-118">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="257df-118">**audioFormat**</span></span>           | <span data-ttu-id="257df-119">string</span><span class="sxs-lookup"><span data-stu-id="257df-119">string</span></span> | <span data-ttu-id="257df-120">Название формата аудио (AAC, MP3, и т. д.).</span><span class="sxs-lookup"><span data-stu-id="257df-120">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="257df-121">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="257df-121">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="257df-122">Int32</span><span class="sxs-lookup"><span data-stu-id="257df-122">Int32</span></span>  | <span data-ttu-id="257df-123">Количество выборок звука в секунду.</span><span class="sxs-lookup"><span data-stu-id="257df-123">Number of audio samples per second.</span></span>
| <span data-ttu-id="257df-124">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="257df-124">**bitrate**</span></span>               | <span data-ttu-id="257df-125">Int32</span><span class="sxs-lookup"><span data-stu-id="257df-125">Int32</span></span>  | <span data-ttu-id="257df-126">Скорость видео в битах в секунду.</span><span class="sxs-lookup"><span data-stu-id="257df-126">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="257df-127">**duration**</span><span class="sxs-lookup"><span data-stu-id="257df-127">**duration**</span></span>              | <span data-ttu-id="257df-128">Int64</span><span class="sxs-lookup"><span data-stu-id="257df-128">Int64</span></span>  | <span data-ttu-id="257df-129">Длительность файла в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="257df-129">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="257df-130">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="257df-130">**fourCC**</span></span>                | <span data-ttu-id="257df-131">string</span><span class="sxs-lookup"><span data-stu-id="257df-131">string</span></span> | <span data-ttu-id="257df-132">Название формата видео в виде четырехзначного кода.</span><span class="sxs-lookup"><span data-stu-id="257df-132">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="257df-133">**framerate**</span><span class="sxs-lookup"><span data-stu-id="257df-133">**framerate**</span></span>             | <span data-ttu-id="257df-134">double</span><span class="sxs-lookup"><span data-stu-id="257df-134">double</span></span> | <span data-ttu-id="257df-135">Частота кадров видео.</span><span class="sxs-lookup"><span data-stu-id="257df-135">Frame rate of the video.</span></span>
| <span data-ttu-id="257df-136">**height**</span><span class="sxs-lookup"><span data-stu-id="257df-136">**height**</span></span>                | <span data-ttu-id="257df-137">Int32</span><span class="sxs-lookup"><span data-stu-id="257df-137">Int32</span></span>  | <span data-ttu-id="257df-138">Высота видео в пикселях.</span><span class="sxs-lookup"><span data-stu-id="257df-138">Height of the video, in pixels.</span></span>
| <span data-ttu-id="257df-139">**width**</span><span class="sxs-lookup"><span data-stu-id="257df-139">**width**</span></span>                 | <span data-ttu-id="257df-140">Int32</span><span class="sxs-lookup"><span data-stu-id="257df-140">Int32</span></span>  | <span data-ttu-id="257df-141">Ширина видео в пикселях.</span><span class="sxs-lookup"><span data-stu-id="257df-141">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="257df-142">Заметки</span><span class="sxs-lookup"><span data-stu-id="257df-142">Remarks</span></span>

<span data-ttu-id="257df-143">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="257df-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/video.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
