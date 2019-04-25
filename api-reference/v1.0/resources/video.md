---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Видео
localization_priority: Normal
ms.openlocfilehash: deba8cccb5f0ab80ca03395ef9f798719d542b8d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521847"
---
# <a name="video-resource-type"></a><span data-ttu-id="f978c-102">Тип ресурса video</span><span class="sxs-lookup"><span data-stu-id="f978c-102">Video resource type</span></span>

<span data-ttu-id="f978c-103">Ресурс **Video** — это единая структура, объединяющая элементы данных, связанные с видео.</span><span class="sxs-lookup"><span data-stu-id="f978c-103">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="f978c-p101">Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **video**, то этот ресурс представляет видеофайл. Свойства ресурса **Video** заполняются путем извлечения метаданных из такого файла.</span><span class="sxs-lookup"><span data-stu-id="f978c-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f978c-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f978c-106">JSON representation</span></span>

<span data-ttu-id="f978c-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="f978c-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="f978c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f978c-108">Properties</span></span>

| <span data-ttu-id="f978c-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="f978c-109">Property name</span></span>             | <span data-ttu-id="f978c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f978c-110">Type</span></span>   | <span data-ttu-id="f978c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f978c-111">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="f978c-112">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="f978c-112">**audioBitsPerSample**</span></span>    | <span data-ttu-id="f978c-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f978c-113">Int32</span></span>  | <span data-ttu-id="f978c-114">Количество разрядов звука на выборку.</span><span class="sxs-lookup"><span data-stu-id="f978c-114">Number of audio bits per sample.</span></span>
| <span data-ttu-id="f978c-115">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="f978c-115">**audioChannels**</span></span>         | <span data-ttu-id="f978c-116">Int32</span><span class="sxs-lookup"><span data-stu-id="f978c-116">Int32</span></span>  | <span data-ttu-id="f978c-117">Количество звуковых каналов.</span><span class="sxs-lookup"><span data-stu-id="f978c-117">Number of audio channels.</span></span>
| <span data-ttu-id="f978c-118">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="f978c-118">**audioFormat**</span></span>           | <span data-ttu-id="f978c-119">string</span><span class="sxs-lookup"><span data-stu-id="f978c-119">string</span></span> | <span data-ttu-id="f978c-120">Название формата аудио (AAC, MP3, и т. д.).</span><span class="sxs-lookup"><span data-stu-id="f978c-120">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="f978c-121">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="f978c-121">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="f978c-122">Int32</span><span class="sxs-lookup"><span data-stu-id="f978c-122">Int32</span></span>  | <span data-ttu-id="f978c-123">Количество выборок звука в секунду.</span><span class="sxs-lookup"><span data-stu-id="f978c-123">Number of audio samples per second.</span></span>
| <span data-ttu-id="f978c-124">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="f978c-124">**bitrate**</span></span>               | <span data-ttu-id="f978c-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f978c-125">Int32</span></span>  | <span data-ttu-id="f978c-126">Скорость видео в битах в секунду.</span><span class="sxs-lookup"><span data-stu-id="f978c-126">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="f978c-127">**duration**</span><span class="sxs-lookup"><span data-stu-id="f978c-127">**duration**</span></span>              | <span data-ttu-id="f978c-128">Int64</span><span class="sxs-lookup"><span data-stu-id="f978c-128">Int64</span></span>  | <span data-ttu-id="f978c-129">Длительность файла в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="f978c-129">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="f978c-130">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="f978c-130">**fourCC**</span></span>                | <span data-ttu-id="f978c-131">string</span><span class="sxs-lookup"><span data-stu-id="f978c-131">string</span></span> | <span data-ttu-id="f978c-132">Название формата видео в виде четырехзначного кода.</span><span class="sxs-lookup"><span data-stu-id="f978c-132">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="f978c-133">**Частота**</span><span class="sxs-lookup"><span data-stu-id="f978c-133">**frameRate**</span></span>             | <span data-ttu-id="f978c-134">double</span><span class="sxs-lookup"><span data-stu-id="f978c-134">double</span></span> | <span data-ttu-id="f978c-135">Частота кадров видео.</span><span class="sxs-lookup"><span data-stu-id="f978c-135">Frame rate of the video.</span></span>
| <span data-ttu-id="f978c-136">**height**</span><span class="sxs-lookup"><span data-stu-id="f978c-136">**height**</span></span>                | <span data-ttu-id="f978c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f978c-137">Int32</span></span>  | <span data-ttu-id="f978c-138">Высота видео в пикселях.</span><span class="sxs-lookup"><span data-stu-id="f978c-138">Height of the video, in pixels.</span></span>
| <span data-ttu-id="f978c-139">**width**</span><span class="sxs-lookup"><span data-stu-id="f978c-139">**width**</span></span>                 | <span data-ttu-id="f978c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f978c-140">Int32</span></span>  | <span data-ttu-id="f978c-141">Ширина видео в пикселях.</span><span class="sxs-lookup"><span data-stu-id="f978c-141">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="f978c-142">Заметки</span><span class="sxs-lookup"><span data-stu-id="f978c-142">Remarks</span></span>

<span data-ttu-id="f978c-143">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f978c-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->
