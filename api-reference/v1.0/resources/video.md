---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Video
ms.openlocfilehash: dd6ece46ce54fe791c0e6b5801287e2abad4fe48
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="video-resource-type"></a><span data-ttu-id="c87cf-102">Тип ресурса Video</span><span class="sxs-lookup"><span data-stu-id="c87cf-102">Video resource type</span></span>

<span data-ttu-id="c87cf-103">Ресурс **Video** — это единая структура, объединяющая элементы данных, связанные с видео.</span><span class="sxs-lookup"><span data-stu-id="c87cf-103">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="c87cf-104">Если у ресурса [**DriveItem**](driveitem.md) есть аспект **video**, значение которого не равно null, то этот ресурс представляет видеофайл.</span><span class="sxs-lookup"><span data-stu-id="c87cf-104">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the Video resource are populated by extracting metadata from the file.</span></span>
<span data-ttu-id="c87cf-105">Свойства ресурса **Video** заполняются путем извлечения метаданных из этого файла.</span><span class="sxs-lookup"><span data-stu-id="c87cf-105">If a DriveItem has a non-null video facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c87cf-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c87cf-106">JSON representation</span></span>

<span data-ttu-id="c87cf-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="c87cf-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="c87cf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c87cf-108">Properties</span></span>

| <span data-ttu-id="c87cf-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c87cf-109">Property name</span></span>             | <span data-ttu-id="c87cf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c87cf-110">Type</span></span>   | <span data-ttu-id="c87cf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c87cf-111">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="c87cf-112">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="c87cf-112">**audioBitsPerSample**</span></span>    | <span data-ttu-id="c87cf-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c87cf-113">Int32</span></span>  | <span data-ttu-id="c87cf-114">Количество разрядов звука на выборку.</span><span class="sxs-lookup"><span data-stu-id="c87cf-114">Number of audio bits per sample.</span></span>
| <span data-ttu-id="c87cf-115">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="c87cf-115">**audioChannels**</span></span>         | <span data-ttu-id="c87cf-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c87cf-116">Int32</span></span>  | <span data-ttu-id="c87cf-117">Количество звуковых каналов.</span><span class="sxs-lookup"><span data-stu-id="c87cf-117">Number of audio channels.</span></span>
| <span data-ttu-id="c87cf-118">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="c87cf-118">**audioFormat**</span></span>           | <span data-ttu-id="c87cf-119">строка</span><span class="sxs-lookup"><span data-stu-id="c87cf-119">string</span></span> | <span data-ttu-id="c87cf-120">Название формата аудио (AAC, MP3, и т. д.).</span><span class="sxs-lookup"><span data-stu-id="c87cf-120">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="c87cf-121">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="c87cf-121">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="c87cf-122">Int32</span><span class="sxs-lookup"><span data-stu-id="c87cf-122">Int32</span></span>  | <span data-ttu-id="c87cf-123">Количество выборок звука в секунду.</span><span class="sxs-lookup"><span data-stu-id="c87cf-123">Number of audio samples per second.</span></span>
| <span data-ttu-id="c87cf-124">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="c87cf-124">**bitrate**</span></span>               | <span data-ttu-id="c87cf-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c87cf-125">Int32</span></span>  | <span data-ttu-id="c87cf-126">Скорость видео в битах в секунду.</span><span class="sxs-lookup"><span data-stu-id="c87cf-126">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="c87cf-127">**duration**</span><span class="sxs-lookup"><span data-stu-id="c87cf-127">**duration**</span></span>              | <span data-ttu-id="c87cf-128">Int64</span><span class="sxs-lookup"><span data-stu-id="c87cf-128">Int64</span></span>  | <span data-ttu-id="c87cf-129">Длительность файла в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="c87cf-129">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="c87cf-130">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="c87cf-130">**fourCC**</span></span>                | <span data-ttu-id="c87cf-131">строка</span><span class="sxs-lookup"><span data-stu-id="c87cf-131">string</span></span> | <span data-ttu-id="c87cf-132">Название формата видео в виде четырехзначного кода.</span><span class="sxs-lookup"><span data-stu-id="c87cf-132">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="c87cf-133">**framerate**</span><span class="sxs-lookup"><span data-stu-id="c87cf-133">**framerate**</span></span>             | <span data-ttu-id="c87cf-134">double</span><span class="sxs-lookup"><span data-stu-id="c87cf-134">double</span></span> | <span data-ttu-id="c87cf-135">Частота кадров видео.</span><span class="sxs-lookup"><span data-stu-id="c87cf-135">Frame rate of the video.</span></span>
| <span data-ttu-id="c87cf-136">**height**</span><span class="sxs-lookup"><span data-stu-id="c87cf-136">**height**</span></span>                | <span data-ttu-id="c87cf-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c87cf-137">Int32</span></span>  | <span data-ttu-id="c87cf-138">Высота видео в пикселях.</span><span class="sxs-lookup"><span data-stu-id="c87cf-138">Height of the video, in pixels.</span></span>
| <span data-ttu-id="c87cf-139">**width**</span><span class="sxs-lookup"><span data-stu-id="c87cf-139">**width**</span></span>                 | <span data-ttu-id="c87cf-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c87cf-140">Int32</span></span>  | <span data-ttu-id="c87cf-141">Ширина видео в пикселях.</span><span class="sxs-lookup"><span data-stu-id="c87cf-141">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="c87cf-142">Заметки</span><span class="sxs-lookup"><span data-stu-id="c87cf-142">Remarks</span></span>

<span data-ttu-id="c87cf-143">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c87cf-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->
