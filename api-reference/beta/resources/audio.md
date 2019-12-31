---
author: ananmishr
description: Ресурс Audio группирует свойства элемента, связанные со звуком, в единую структуру.
ms.date: 09/10/2017
title: "\"Audio\" (Аудио);"
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 539afcd93ed2f8d9d5b1a136edefa5a69fd2e4bd
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913144"
---
# <a name="audio-facet"></a><span data-ttu-id="15c27-103">Аспект Audio</span><span class="sxs-lookup"><span data-stu-id="15c27-103">Audio facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15c27-104">Ресурс **Audio** группирует свойства элемента, связанные со звуком, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="15c27-104">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="15c27-p101">Если у элемента [**DriveItem**](driveitem.md) есть ненулевой аспект **audio**, то этот элемент представляет звуковой файл. Свойства ресурса **Audio** заполняются путем извлечения метаданных из такого файла.</span><span class="sxs-lookup"><span data-stu-id="15c27-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="15c27-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="15c27-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="15c27-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="15c27-108">Properties</span></span>

| <span data-ttu-id="15c27-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="15c27-109">Property name</span></span>         | <span data-ttu-id="15c27-110">Тип</span><span class="sxs-lookup"><span data-stu-id="15c27-110">Type</span></span>    | <span data-ttu-id="15c27-111">Описание</span><span class="sxs-lookup"><span data-stu-id="15c27-111">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="15c27-112">**album**</span><span class="sxs-lookup"><span data-stu-id="15c27-112">**album**</span></span>             | <span data-ttu-id="15c27-113">string</span><span class="sxs-lookup"><span data-stu-id="15c27-113">string</span></span>  | <span data-ttu-id="15c27-114">Название альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="15c27-114">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="15c27-115">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="15c27-115">**albumArtist**</span></span>       | <span data-ttu-id="15c27-116">string</span><span class="sxs-lookup"><span data-stu-id="15c27-116">string</span></span>  | <span data-ttu-id="15c27-117">Название исполнителя альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="15c27-117">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="15c27-118">**artist**</span><span class="sxs-lookup"><span data-stu-id="15c27-118">**artist**</span></span>            | <span data-ttu-id="15c27-119">string</span><span class="sxs-lookup"><span data-stu-id="15c27-119">string</span></span>  | <span data-ttu-id="15c27-120">Исполнитель для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="15c27-120">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="15c27-121">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="15c27-121">**bitrate**</span></span>           | <span data-ttu-id="15c27-122">Int32</span><span class="sxs-lookup"><span data-stu-id="15c27-122">Int32</span></span>   | <span data-ttu-id="15c27-123">Скорость передачи данных в кбит/с.</span><span class="sxs-lookup"><span data-stu-id="15c27-123">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="15c27-124">**composers**</span><span class="sxs-lookup"><span data-stu-id="15c27-124">**composers**</span></span>         | <span data-ttu-id="15c27-125">string</span><span class="sxs-lookup"><span data-stu-id="15c27-125">string</span></span>  | <span data-ttu-id="15c27-126">Имя композитора для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="15c27-126">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="15c27-127">**copyright**</span><span class="sxs-lookup"><span data-stu-id="15c27-127">**copyright**</span></span>         | <span data-ttu-id="15c27-128">string</span><span class="sxs-lookup"><span data-stu-id="15c27-128">string</span></span>  | <span data-ttu-id="15c27-129">Сведения об авторском праве для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="15c27-129">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="15c27-130">**disc**</span><span class="sxs-lookup"><span data-stu-id="15c27-130">**disc**</span></span>              | <span data-ttu-id="15c27-131">Int32</span><span class="sxs-lookup"><span data-stu-id="15c27-131">Int32</span></span>   | <span data-ttu-id="15c27-132">Номер диска, с которого был взят этот звуковой файл.</span><span class="sxs-lookup"><span data-stu-id="15c27-132">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="15c27-133">**discCount**</span><span class="sxs-lookup"><span data-stu-id="15c27-133">**discCount**</span></span>         | <span data-ttu-id="15c27-134">Int32</span><span class="sxs-lookup"><span data-stu-id="15c27-134">Int32</span></span>   | <span data-ttu-id="15c27-135">Общее количество дисков для этого альбома.</span><span class="sxs-lookup"><span data-stu-id="15c27-135">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="15c27-136">**duration**</span><span class="sxs-lookup"><span data-stu-id="15c27-136">**duration**</span></span>          | <span data-ttu-id="15c27-137">Int64</span><span class="sxs-lookup"><span data-stu-id="15c27-137">Int64</span></span>   | <span data-ttu-id="15c27-138">Длительность воспроизведения звукового файла в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="15c27-138">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="15c27-139">**genre**</span><span class="sxs-lookup"><span data-stu-id="15c27-139">**genre**</span></span>             | <span data-ttu-id="15c27-140">string</span><span class="sxs-lookup"><span data-stu-id="15c27-140">string</span></span>  | <span data-ttu-id="15c27-141">Жанр этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="15c27-141">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="15c27-142">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="15c27-142">**hasDrm**</span></span>            | <span data-ttu-id="15c27-143">boolean</span><span class="sxs-lookup"><span data-stu-id="15c27-143">boolean</span></span> | <span data-ttu-id="15c27-144">Указывает, защищен ли файл с помощью технологии управления цифровыми правами.</span><span class="sxs-lookup"><span data-stu-id="15c27-144">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="15c27-145">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="15c27-145">**isVariableBitrate**</span></span> | <span data-ttu-id="15c27-146">boolean</span><span class="sxs-lookup"><span data-stu-id="15c27-146">boolean</span></span> | <span data-ttu-id="15c27-147">Указывает, закодирован ли файл с использованием переменной скорости передачи данных.</span><span class="sxs-lookup"><span data-stu-id="15c27-147">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="15c27-148">**title**</span><span class="sxs-lookup"><span data-stu-id="15c27-148">**title**</span></span>             | <span data-ttu-id="15c27-149">строка</span><span class="sxs-lookup"><span data-stu-id="15c27-149">string</span></span>  | <span data-ttu-id="15c27-150">Название звукового файла.</span><span class="sxs-lookup"><span data-stu-id="15c27-150">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="15c27-151">**track**</span><span class="sxs-lookup"><span data-stu-id="15c27-151">**track**</span></span>             | <span data-ttu-id="15c27-152">Int32</span><span class="sxs-lookup"><span data-stu-id="15c27-152">Int32</span></span>   | <span data-ttu-id="15c27-153">Номер дорожки на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="15c27-153">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="15c27-154">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="15c27-154">**trackCount**</span></span>        | <span data-ttu-id="15c27-155">Int32</span><span class="sxs-lookup"><span data-stu-id="15c27-155">Int32</span></span>   | <span data-ttu-id="15c27-156">Общее количество дорожек на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="15c27-156">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="15c27-157">**year**</span><span class="sxs-lookup"><span data-stu-id="15c27-157">**year**</span></span>              | <span data-ttu-id="15c27-158">Int32</span><span class="sxs-lookup"><span data-stu-id="15c27-158">Int32</span></span>   | <span data-ttu-id="15c27-159">Год записи звукового файла.</span><span class="sxs-lookup"><span data-stu-id="15c27-159">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="15c27-160">Примечания</span><span class="sxs-lookup"><span data-stu-id="15c27-160">Remarks</span></span>

<span data-ttu-id="15c27-161">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="15c27-161">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
