---
author: ananmishr
description: Ресурс Audio группирует свойства элемента, связанные со звуком, в единую структуру.
ms.date: 09/10/2017
title: "\"Audio\" (Аудио);"
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 944ad03a3ab70be5131e64f7d96c2a14ffea06ea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508131"
---
# <a name="audio-facet"></a><span data-ttu-id="4cb1d-103">Аспект Audio</span><span class="sxs-lookup"><span data-stu-id="4cb1d-103">Audio facet</span></span>

<span data-ttu-id="4cb1d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cb1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cb1d-105">Ресурс **Audio** группирует свойства элемента, связанные со звуком, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="4cb1d-105">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="4cb1d-p101">Если у элемента [**DriveItem**](driveitem.md) есть ненулевой аспект **audio**, то этот элемент представляет звуковой файл. Свойства ресурса **Audio** заполняются путем извлечения метаданных из такого файла.</span><span class="sxs-lookup"><span data-stu-id="4cb1d-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="4cb1d-108">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4cb1d-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.audio" } -->
```json
{
  "album": "string",
  "albumArtist": "string",
  "artist": "string",
  "bitrate": 128,
  "composers": "string",
  "copyright": "string",
  "disc": 0,
  "discCount": 0,
  "duration": 567,
  "genre": "string",
  "hasDrm": false,
  "isVariableBitrate": false,
  "title": "string",
  "track": 1,
  "trackCount": 16,
  "year": 2014
}
```

## <a name="properties"></a><span data-ttu-id="4cb1d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4cb1d-109">Properties</span></span>

| <span data-ttu-id="4cb1d-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="4cb1d-110">Property name</span></span>         | <span data-ttu-id="4cb1d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4cb1d-111">Type</span></span>    | <span data-ttu-id="4cb1d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4cb1d-112">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="4cb1d-113">**album**</span><span class="sxs-lookup"><span data-stu-id="4cb1d-113">**album**</span></span>             | <span data-ttu-id="4cb1d-114">string</span><span class="sxs-lookup"><span data-stu-id="4cb1d-114">string</span></span>  | <span data-ttu-id="4cb1d-115">Название альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4cb1d-115">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="4cb1d-116">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="4cb1d-116">**albumArtist**</span></span>       | <span data-ttu-id="4cb1d-117">string</span><span class="sxs-lookup"><span data-stu-id="4cb1d-117">string</span></span>  | <span data-ttu-id="4cb1d-118">Название исполнителя альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4cb1d-118">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="4cb1d-119">**artist**</span><span class="sxs-lookup"><span data-stu-id="4cb1d-119">**artist**</span></span>            | <span data-ttu-id="4cb1d-120">string</span><span class="sxs-lookup"><span data-stu-id="4cb1d-120">string</span></span>  | <span data-ttu-id="4cb1d-121">Исполнитель для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4cb1d-121">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="4cb1d-122">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="4cb1d-122">**bitrate**</span></span>           | <span data-ttu-id="4cb1d-123">Int32</span><span class="sxs-lookup"><span data-stu-id="4cb1d-123">Int32</span></span>   | <span data-ttu-id="4cb1d-124">Скорость передачи данных в кбит/с.</span><span class="sxs-lookup"><span data-stu-id="4cb1d-124">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="4cb1d-125">**composers**</span><span class="sxs-lookup"><span data-stu-id="4cb1d-125">**composers**</span></span>         | <span data-ttu-id="4cb1d-126">string</span><span class="sxs-lookup"><span data-stu-id="4cb1d-126">string</span></span>  | <span data-ttu-id="4cb1d-127">Имя композитора для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4cb1d-127">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="4cb1d-128">**copyright**</span><span class="sxs-lookup"><span data-stu-id="4cb1d-128">**copyright**</span></span>         | <span data-ttu-id="4cb1d-129">string</span><span class="sxs-lookup"><span data-stu-id="4cb1d-129">string</span></span>  | <span data-ttu-id="4cb1d-130">Сведения об авторском праве для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4cb1d-130">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="4cb1d-131">**disc**</span><span class="sxs-lookup"><span data-stu-id="4cb1d-131">**disc**</span></span>              | <span data-ttu-id="4cb1d-132">Int32</span><span class="sxs-lookup"><span data-stu-id="4cb1d-132">Int32</span></span>   | <span data-ttu-id="4cb1d-133">Номер диска, с которого был взят этот звуковой файл.</span><span class="sxs-lookup"><span data-stu-id="4cb1d-133">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="4cb1d-134">**discCount**</span><span class="sxs-lookup"><span data-stu-id="4cb1d-134">**discCount**</span></span>         | <span data-ttu-id="4cb1d-135">Int32</span><span class="sxs-lookup"><span data-stu-id="4cb1d-135">Int32</span></span>   | <span data-ttu-id="4cb1d-136">Общее количество дисков для этого альбома.</span><span class="sxs-lookup"><span data-stu-id="4cb1d-136">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="4cb1d-137">**duration**</span><span class="sxs-lookup"><span data-stu-id="4cb1d-137">**duration**</span></span>          | <span data-ttu-id="4cb1d-138">Int64</span><span class="sxs-lookup"><span data-stu-id="4cb1d-138">Int64</span></span>   | <span data-ttu-id="4cb1d-139">Длительность воспроизведения звукового файла в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="4cb1d-139">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="4cb1d-140">**genre**</span><span class="sxs-lookup"><span data-stu-id="4cb1d-140">**genre**</span></span>             | <span data-ttu-id="4cb1d-141">string</span><span class="sxs-lookup"><span data-stu-id="4cb1d-141">string</span></span>  | <span data-ttu-id="4cb1d-142">Жанр этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4cb1d-142">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="4cb1d-143">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="4cb1d-143">**hasDrm**</span></span>            | <span data-ttu-id="4cb1d-144">boolean</span><span class="sxs-lookup"><span data-stu-id="4cb1d-144">boolean</span></span> | <span data-ttu-id="4cb1d-145">Указывает, защищен ли файл с помощью технологии управления цифровыми правами.</span><span class="sxs-lookup"><span data-stu-id="4cb1d-145">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="4cb1d-146">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="4cb1d-146">**isVariableBitrate**</span></span> | <span data-ttu-id="4cb1d-147">boolean</span><span class="sxs-lookup"><span data-stu-id="4cb1d-147">boolean</span></span> | <span data-ttu-id="4cb1d-148">Указывает, закодирован ли файл с использованием переменной скорости передачи данных.</span><span class="sxs-lookup"><span data-stu-id="4cb1d-148">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="4cb1d-149">**title**</span><span class="sxs-lookup"><span data-stu-id="4cb1d-149">**title**</span></span>             | <span data-ttu-id="4cb1d-150">строка</span><span class="sxs-lookup"><span data-stu-id="4cb1d-150">string</span></span>  | <span data-ttu-id="4cb1d-151">Название звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4cb1d-151">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="4cb1d-152">**track**</span><span class="sxs-lookup"><span data-stu-id="4cb1d-152">**track**</span></span>             | <span data-ttu-id="4cb1d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="4cb1d-153">Int32</span></span>   | <span data-ttu-id="4cb1d-154">Номер дорожки на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4cb1d-154">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="4cb1d-155">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="4cb1d-155">**trackCount**</span></span>        | <span data-ttu-id="4cb1d-156">Int32</span><span class="sxs-lookup"><span data-stu-id="4cb1d-156">Int32</span></span>   | <span data-ttu-id="4cb1d-157">Общее количество дорожек на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4cb1d-157">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="4cb1d-158">**year**</span><span class="sxs-lookup"><span data-stu-id="4cb1d-158">**year**</span></span>              | <span data-ttu-id="4cb1d-159">Int32</span><span class="sxs-lookup"><span data-stu-id="4cb1d-159">Int32</span></span>   | <span data-ttu-id="4cb1d-160">Год записи звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4cb1d-160">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="4cb1d-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="4cb1d-161">Remarks</span></span>

<span data-ttu-id="4cb1d-162">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="4cb1d-162">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio",
  "suppressions": []
}
-->
