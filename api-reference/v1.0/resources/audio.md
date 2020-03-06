---
author: ananmishr
ms.date: 09/10/2017
title: "\"Audio\" (Аудио);"
localization_priority: Normal
ms.prod: microsoft-teams
description: Ресурс Audio группирует свойства элемента, связанные со звуком, в единую структуру.
doc_type: resourcePageType
ms.openlocfilehash: 5487c7fb0505a1ab9a6b0e53278e235083cb83e4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532065"
---
# <a name="audio-facet"></a><span data-ttu-id="2d958-103">Аспект Audio</span><span class="sxs-lookup"><span data-stu-id="2d958-103">Audio facet</span></span>

<span data-ttu-id="2d958-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d958-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d958-105">Ресурс **Audio** группирует свойства элемента, связанные со звуком, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="2d958-105">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="2d958-p101">Если у элемента [**DriveItem**](driveitem.md) есть ненулевой аспект **audio**, то этот элемент представляет звуковой файл. Свойства ресурса **Audio** заполняются путем извлечения метаданных из такого файла.</span><span class="sxs-lookup"><span data-stu-id="2d958-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="2d958-108">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2d958-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2d958-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d958-109">Properties</span></span>

| <span data-ttu-id="2d958-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2d958-110">Property name</span></span>         | <span data-ttu-id="2d958-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2d958-111">Type</span></span>    | <span data-ttu-id="2d958-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2d958-112">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="2d958-113">**album**</span><span class="sxs-lookup"><span data-stu-id="2d958-113">**album**</span></span>             | <span data-ttu-id="2d958-114">string</span><span class="sxs-lookup"><span data-stu-id="2d958-114">string</span></span>  | <span data-ttu-id="2d958-115">Название альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="2d958-115">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="2d958-116">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="2d958-116">**albumArtist**</span></span>       | <span data-ttu-id="2d958-117">string</span><span class="sxs-lookup"><span data-stu-id="2d958-117">string</span></span>  | <span data-ttu-id="2d958-118">Название исполнителя альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="2d958-118">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="2d958-119">**artist**</span><span class="sxs-lookup"><span data-stu-id="2d958-119">**artist**</span></span>            | <span data-ttu-id="2d958-120">string</span><span class="sxs-lookup"><span data-stu-id="2d958-120">string</span></span>  | <span data-ttu-id="2d958-121">Исполнитель для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="2d958-121">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="2d958-122">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="2d958-122">**bitrate**</span></span>           | <span data-ttu-id="2d958-123">Int64</span><span class="sxs-lookup"><span data-stu-id="2d958-123">Int64</span></span>   | <span data-ttu-id="2d958-124">Скорость передачи данных в кбит/с.</span><span class="sxs-lookup"><span data-stu-id="2d958-124">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="2d958-125">**composers**</span><span class="sxs-lookup"><span data-stu-id="2d958-125">**composers**</span></span>         | <span data-ttu-id="2d958-126">string</span><span class="sxs-lookup"><span data-stu-id="2d958-126">string</span></span>  | <span data-ttu-id="2d958-127">Имя композитора для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="2d958-127">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="2d958-128">**copyright**</span><span class="sxs-lookup"><span data-stu-id="2d958-128">**copyright**</span></span>         | <span data-ttu-id="2d958-129">string</span><span class="sxs-lookup"><span data-stu-id="2d958-129">string</span></span>  | <span data-ttu-id="2d958-130">Сведения об авторском праве для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="2d958-130">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="2d958-131">**disc**</span><span class="sxs-lookup"><span data-stu-id="2d958-131">**disc**</span></span>              | <span data-ttu-id="2d958-132">Int16</span><span class="sxs-lookup"><span data-stu-id="2d958-132">Int16</span></span>   | <span data-ttu-id="2d958-133">Номер диска, с которого был взят этот звуковой файл.</span><span class="sxs-lookup"><span data-stu-id="2d958-133">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="2d958-134">**discCount**</span><span class="sxs-lookup"><span data-stu-id="2d958-134">**discCount**</span></span>         | <span data-ttu-id="2d958-135">Int16</span><span class="sxs-lookup"><span data-stu-id="2d958-135">Int16</span></span>   | <span data-ttu-id="2d958-136">Общее количество дисков для этого альбома.</span><span class="sxs-lookup"><span data-stu-id="2d958-136">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="2d958-137">**duration**</span><span class="sxs-lookup"><span data-stu-id="2d958-137">**duration**</span></span>          | <span data-ttu-id="2d958-138">Int64</span><span class="sxs-lookup"><span data-stu-id="2d958-138">Int64</span></span>   | <span data-ttu-id="2d958-139">Длительность воспроизведения звукового файла в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="2d958-139">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="2d958-140">**genre**</span><span class="sxs-lookup"><span data-stu-id="2d958-140">**genre**</span></span>             | <span data-ttu-id="2d958-141">string</span><span class="sxs-lookup"><span data-stu-id="2d958-141">string</span></span>  | <span data-ttu-id="2d958-142">Жанр этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="2d958-142">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="2d958-143">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="2d958-143">**hasDrm**</span></span>            | <span data-ttu-id="2d958-144">boolean</span><span class="sxs-lookup"><span data-stu-id="2d958-144">boolean</span></span> | <span data-ttu-id="2d958-145">Указывает, защищен ли файл с помощью технологии управления цифровыми правами.</span><span class="sxs-lookup"><span data-stu-id="2d958-145">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="2d958-146">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="2d958-146">**isVariableBitrate**</span></span> | <span data-ttu-id="2d958-147">boolean</span><span class="sxs-lookup"><span data-stu-id="2d958-147">boolean</span></span> | <span data-ttu-id="2d958-148">Указывает, закодирован ли файл с использованием переменной скорости передачи данных.</span><span class="sxs-lookup"><span data-stu-id="2d958-148">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="2d958-149">**title**</span><span class="sxs-lookup"><span data-stu-id="2d958-149">**title**</span></span>             | <span data-ttu-id="2d958-150">строка</span><span class="sxs-lookup"><span data-stu-id="2d958-150">string</span></span>  | <span data-ttu-id="2d958-151">Название звукового файла.</span><span class="sxs-lookup"><span data-stu-id="2d958-151">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="2d958-152">**track**</span><span class="sxs-lookup"><span data-stu-id="2d958-152">**track**</span></span>             | <span data-ttu-id="2d958-153">Int32</span><span class="sxs-lookup"><span data-stu-id="2d958-153">Int32</span></span>   | <span data-ttu-id="2d958-154">Номер дорожки на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="2d958-154">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="2d958-155">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="2d958-155">**trackCount**</span></span>        | <span data-ttu-id="2d958-156">Int32</span><span class="sxs-lookup"><span data-stu-id="2d958-156">Int32</span></span>   | <span data-ttu-id="2d958-157">Общее количество дорожек на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="2d958-157">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="2d958-158">**year**</span><span class="sxs-lookup"><span data-stu-id="2d958-158">**year**</span></span>              | <span data-ttu-id="2d958-159">Int32</span><span class="sxs-lookup"><span data-stu-id="2d958-159">Int32</span></span>   | <span data-ttu-id="2d958-160">Год записи звукового файла.</span><span class="sxs-lookup"><span data-stu-id="2d958-160">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="2d958-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="2d958-161">Remarks</span></span>

<span data-ttu-id="2d958-162">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="2d958-162">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
