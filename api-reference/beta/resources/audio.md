---
author: VinodRavichandran
ms.date: 09/10/2017
title: Audio
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b4ff9e98b3024184298da144f90665ba2f192fef
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642277"
---
# <a name="audio-facet"></a><span data-ttu-id="0bbc2-102">Аспект Audio</span><span class="sxs-lookup"><span data-stu-id="0bbc2-102">Audio facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bbc2-103">Ресурс **Audio** группирует свойства элемента, связанные со звуком, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="0bbc2-103">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="0bbc2-p101">Если у элемента [**DriveItem**](driveitem.md) есть ненулевой аспект **audio**, то этот элемент представляет звуковой файл. Свойства ресурса **Audio** заполняются путем извлечения метаданных из такого файла.</span><span class="sxs-lookup"><span data-stu-id="0bbc2-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="0bbc2-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0bbc2-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0bbc2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0bbc2-107">Properties</span></span>

| <span data-ttu-id="0bbc2-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="0bbc2-108">Property name</span></span>         | <span data-ttu-id="0bbc2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0bbc2-109">Type</span></span>    | <span data-ttu-id="0bbc2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0bbc2-110">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="0bbc2-111">**album**</span><span class="sxs-lookup"><span data-stu-id="0bbc2-111">**album**</span></span>             | <span data-ttu-id="0bbc2-112">строка</span><span class="sxs-lookup"><span data-stu-id="0bbc2-112">string</span></span>  | <span data-ttu-id="0bbc2-113">Название альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="0bbc2-113">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="0bbc2-114">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="0bbc2-114">**albumArtist**</span></span>       | <span data-ttu-id="0bbc2-115">строка</span><span class="sxs-lookup"><span data-stu-id="0bbc2-115">string</span></span>  | <span data-ttu-id="0bbc2-116">Название исполнителя альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="0bbc2-116">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="0bbc2-117">**artist**</span><span class="sxs-lookup"><span data-stu-id="0bbc2-117">**artist**</span></span>            | <span data-ttu-id="0bbc2-118">строка</span><span class="sxs-lookup"><span data-stu-id="0bbc2-118">string</span></span>  | <span data-ttu-id="0bbc2-119">Исполнитель для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="0bbc2-119">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="0bbc2-120">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="0bbc2-120">**bitrate**</span></span>           | <span data-ttu-id="0bbc2-121">Int32</span><span class="sxs-lookup"><span data-stu-id="0bbc2-121">Int32</span></span>   | <span data-ttu-id="0bbc2-122">Скорость передачи данных в кбит/с.</span><span class="sxs-lookup"><span data-stu-id="0bbc2-122">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="0bbc2-123">**composers**</span><span class="sxs-lookup"><span data-stu-id="0bbc2-123">**composers**</span></span>         | <span data-ttu-id="0bbc2-124">строка</span><span class="sxs-lookup"><span data-stu-id="0bbc2-124">string</span></span>  | <span data-ttu-id="0bbc2-125">Имя композитора для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="0bbc2-125">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="0bbc2-126">**copyright**</span><span class="sxs-lookup"><span data-stu-id="0bbc2-126">**copyright**</span></span>         | <span data-ttu-id="0bbc2-127">строка</span><span class="sxs-lookup"><span data-stu-id="0bbc2-127">string</span></span>  | <span data-ttu-id="0bbc2-128">Сведения об авторском праве для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="0bbc2-128">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="0bbc2-129">**disc**</span><span class="sxs-lookup"><span data-stu-id="0bbc2-129">**disc**</span></span>              | <span data-ttu-id="0bbc2-130">Int32</span><span class="sxs-lookup"><span data-stu-id="0bbc2-130">Int32</span></span>   | <span data-ttu-id="0bbc2-131">Номер диска, с которого был взят этот звуковой файл.</span><span class="sxs-lookup"><span data-stu-id="0bbc2-131">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="0bbc2-132">**discCount**</span><span class="sxs-lookup"><span data-stu-id="0bbc2-132">**discCount**</span></span>         | <span data-ttu-id="0bbc2-133">Int32</span><span class="sxs-lookup"><span data-stu-id="0bbc2-133">Int32</span></span>   | <span data-ttu-id="0bbc2-134">Общее количество дисков для этого альбома.</span><span class="sxs-lookup"><span data-stu-id="0bbc2-134">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="0bbc2-135">**duration**</span><span class="sxs-lookup"><span data-stu-id="0bbc2-135">**duration**</span></span>          | <span data-ttu-id="0bbc2-136">Int64</span><span class="sxs-lookup"><span data-stu-id="0bbc2-136">Int64</span></span>   | <span data-ttu-id="0bbc2-137">Длительность воспроизведения звукового файла в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="0bbc2-137">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="0bbc2-138">**genre**</span><span class="sxs-lookup"><span data-stu-id="0bbc2-138">**genre**</span></span>             | <span data-ttu-id="0bbc2-139">строка</span><span class="sxs-lookup"><span data-stu-id="0bbc2-139">string</span></span>  | <span data-ttu-id="0bbc2-140">Жанр этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="0bbc2-140">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="0bbc2-141">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="0bbc2-141">**hasDrm**</span></span>            | <span data-ttu-id="0bbc2-142">boolean</span><span class="sxs-lookup"><span data-stu-id="0bbc2-142">boolean</span></span> | <span data-ttu-id="0bbc2-143">Указывает, защищен ли файл с помощью технологии управления цифровыми правами.</span><span class="sxs-lookup"><span data-stu-id="0bbc2-143">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="0bbc2-144">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="0bbc2-144">**isVariableBitrate**</span></span> | <span data-ttu-id="0bbc2-145">boolean</span><span class="sxs-lookup"><span data-stu-id="0bbc2-145">boolean</span></span> | <span data-ttu-id="0bbc2-146">Указывает, закодирован ли файл с использованием переменной скорости передачи данных.</span><span class="sxs-lookup"><span data-stu-id="0bbc2-146">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="0bbc2-147">**title**</span><span class="sxs-lookup"><span data-stu-id="0bbc2-147">**title**</span></span>             | <span data-ttu-id="0bbc2-148">строка</span><span class="sxs-lookup"><span data-stu-id="0bbc2-148">string</span></span>  | <span data-ttu-id="0bbc2-149">Название звукового файла.</span><span class="sxs-lookup"><span data-stu-id="0bbc2-149">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="0bbc2-150">**track**</span><span class="sxs-lookup"><span data-stu-id="0bbc2-150">**track**</span></span>             | <span data-ttu-id="0bbc2-151">Int32</span><span class="sxs-lookup"><span data-stu-id="0bbc2-151">Int32</span></span>   | <span data-ttu-id="0bbc2-152">Номер дорожки на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="0bbc2-152">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="0bbc2-153">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="0bbc2-153">**trackCount**</span></span>        | <span data-ttu-id="0bbc2-154">Int32</span><span class="sxs-lookup"><span data-stu-id="0bbc2-154">Int32</span></span>   | <span data-ttu-id="0bbc2-155">Общее количество дорожек на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="0bbc2-155">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="0bbc2-156">**year**</span><span class="sxs-lookup"><span data-stu-id="0bbc2-156">**year**</span></span>              | <span data-ttu-id="0bbc2-157">Int32</span><span class="sxs-lookup"><span data-stu-id="0bbc2-157">Int32</span></span>   | <span data-ttu-id="0bbc2-158">Год записи звукового файла.</span><span class="sxs-lookup"><span data-stu-id="0bbc2-158">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="0bbc2-159">Примечания</span><span class="sxs-lookup"><span data-stu-id="0bbc2-159">Remarks</span></span>

<span data-ttu-id="0bbc2-160">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0bbc2-160">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio",
  "suppressions": [
    "Error: /api-reference/beta/resources/audio.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
