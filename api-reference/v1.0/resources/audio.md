---
author: VinodRavichandran
ms.date: 09/10/2017
title: "\"Audio\" (Аудио);"
localization_priority: Normal
ms.prod: microsoft-teams
description: Ресурс Audio группирует свойства элемента, связанные со звуком, в единую структуру.
doc_type: resourcePageType
ms.openlocfilehash: a71b9ee9c65bacc802244bda2e7757e87d9ff35e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030025"
---
# <a name="audio-facet"></a><span data-ttu-id="59612-103">Аспект Audio</span><span class="sxs-lookup"><span data-stu-id="59612-103">Audio facet</span></span>

<span data-ttu-id="59612-104">Ресурс **Audio** группирует свойства элемента, связанные со звуком, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="59612-104">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="59612-p101">Если у элемента [**DriveItem**](driveitem.md) есть ненулевой аспект **audio**, то этот элемент представляет звуковой файл. Свойства ресурса **Audio** заполняются путем извлечения метаданных из такого файла.</span><span class="sxs-lookup"><span data-stu-id="59612-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="59612-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="59612-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="59612-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="59612-108">Properties</span></span>

| <span data-ttu-id="59612-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="59612-109">Property name</span></span>         | <span data-ttu-id="59612-110">Тип</span><span class="sxs-lookup"><span data-stu-id="59612-110">Type</span></span>    | <span data-ttu-id="59612-111">Описание</span><span class="sxs-lookup"><span data-stu-id="59612-111">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="59612-112">**album**</span><span class="sxs-lookup"><span data-stu-id="59612-112">**album**</span></span>             | <span data-ttu-id="59612-113">string</span><span class="sxs-lookup"><span data-stu-id="59612-113">string</span></span>  | <span data-ttu-id="59612-114">Название альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="59612-114">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="59612-115">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="59612-115">**albumArtist**</span></span>       | <span data-ttu-id="59612-116">string</span><span class="sxs-lookup"><span data-stu-id="59612-116">string</span></span>  | <span data-ttu-id="59612-117">Название исполнителя альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="59612-117">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="59612-118">**artist**</span><span class="sxs-lookup"><span data-stu-id="59612-118">**artist**</span></span>            | <span data-ttu-id="59612-119">string</span><span class="sxs-lookup"><span data-stu-id="59612-119">string</span></span>  | <span data-ttu-id="59612-120">Исполнитель для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="59612-120">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="59612-121">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="59612-121">**bitrate**</span></span>           | <span data-ttu-id="59612-122">Int64</span><span class="sxs-lookup"><span data-stu-id="59612-122">Int64</span></span>   | <span data-ttu-id="59612-123">Скорость передачи данных в кбит/с.</span><span class="sxs-lookup"><span data-stu-id="59612-123">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="59612-124">**composers**</span><span class="sxs-lookup"><span data-stu-id="59612-124">**composers**</span></span>         | <span data-ttu-id="59612-125">string</span><span class="sxs-lookup"><span data-stu-id="59612-125">string</span></span>  | <span data-ttu-id="59612-126">Имя композитора для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="59612-126">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="59612-127">**copyright**</span><span class="sxs-lookup"><span data-stu-id="59612-127">**copyright**</span></span>         | <span data-ttu-id="59612-128">string</span><span class="sxs-lookup"><span data-stu-id="59612-128">string</span></span>  | <span data-ttu-id="59612-129">Сведения об авторском праве для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="59612-129">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="59612-130">**disc**</span><span class="sxs-lookup"><span data-stu-id="59612-130">**disc**</span></span>              | <span data-ttu-id="59612-131">Int16</span><span class="sxs-lookup"><span data-stu-id="59612-131">Int16</span></span>   | <span data-ttu-id="59612-132">Номер диска, с которого был взят этот звуковой файл.</span><span class="sxs-lookup"><span data-stu-id="59612-132">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="59612-133">**discCount**</span><span class="sxs-lookup"><span data-stu-id="59612-133">**discCount**</span></span>         | <span data-ttu-id="59612-134">Int16</span><span class="sxs-lookup"><span data-stu-id="59612-134">Int16</span></span>   | <span data-ttu-id="59612-135">Общее количество дисков для этого альбома.</span><span class="sxs-lookup"><span data-stu-id="59612-135">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="59612-136">**duration**</span><span class="sxs-lookup"><span data-stu-id="59612-136">**duration**</span></span>          | <span data-ttu-id="59612-137">Int64</span><span class="sxs-lookup"><span data-stu-id="59612-137">Int64</span></span>   | <span data-ttu-id="59612-138">Длительность воспроизведения звукового файла в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="59612-138">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="59612-139">**genre**</span><span class="sxs-lookup"><span data-stu-id="59612-139">**genre**</span></span>             | <span data-ttu-id="59612-140">string</span><span class="sxs-lookup"><span data-stu-id="59612-140">string</span></span>  | <span data-ttu-id="59612-141">Жанр этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="59612-141">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="59612-142">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="59612-142">**hasDrm**</span></span>            | <span data-ttu-id="59612-143">boolean</span><span class="sxs-lookup"><span data-stu-id="59612-143">boolean</span></span> | <span data-ttu-id="59612-144">Указывает, защищен ли файл с помощью технологии управления цифровыми правами.</span><span class="sxs-lookup"><span data-stu-id="59612-144">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="59612-145">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="59612-145">**isVariableBitrate**</span></span> | <span data-ttu-id="59612-146">boolean</span><span class="sxs-lookup"><span data-stu-id="59612-146">boolean</span></span> | <span data-ttu-id="59612-147">Указывает, закодирован ли файл с использованием переменной скорости передачи данных.</span><span class="sxs-lookup"><span data-stu-id="59612-147">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="59612-148">**title**</span><span class="sxs-lookup"><span data-stu-id="59612-148">**title**</span></span>             | <span data-ttu-id="59612-149">строка</span><span class="sxs-lookup"><span data-stu-id="59612-149">string</span></span>  | <span data-ttu-id="59612-150">Название звукового файла.</span><span class="sxs-lookup"><span data-stu-id="59612-150">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="59612-151">**track**</span><span class="sxs-lookup"><span data-stu-id="59612-151">**track**</span></span>             | <span data-ttu-id="59612-152">Int32</span><span class="sxs-lookup"><span data-stu-id="59612-152">Int32</span></span>   | <span data-ttu-id="59612-153">Номер дорожки на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="59612-153">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="59612-154">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="59612-154">**trackCount**</span></span>        | <span data-ttu-id="59612-155">Int32</span><span class="sxs-lookup"><span data-stu-id="59612-155">Int32</span></span>   | <span data-ttu-id="59612-156">Общее количество дорожек на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="59612-156">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="59612-157">**year**</span><span class="sxs-lookup"><span data-stu-id="59612-157">**year**</span></span>              | <span data-ttu-id="59612-158">Int32</span><span class="sxs-lookup"><span data-stu-id="59612-158">Int32</span></span>   | <span data-ttu-id="59612-159">Год записи звукового файла.</span><span class="sxs-lookup"><span data-stu-id="59612-159">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="59612-160">Примечания</span><span class="sxs-lookup"><span data-stu-id="59612-160">Remarks</span></span>

<span data-ttu-id="59612-161">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="59612-161">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
