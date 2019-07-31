---
author: VinodRavichandran
description: Ресурс Audio группирует свойства элемента, связанные со звуком, в единую структуру.
ms.date: 09/10/2017
title: "\"Audio\" (Аудио);"
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 078ade2fd92d6eaf8d9017fe5cd8255a7449769e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013229"
---
# <a name="audio-facet"></a><span data-ttu-id="4b562-103">Аспект Audio</span><span class="sxs-lookup"><span data-stu-id="4b562-103">Audio facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b562-104">Ресурс **Audio** группирует свойства элемента, связанные со звуком, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="4b562-104">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="4b562-p101">Если у элемента [**DriveItem**](driveitem.md) есть ненулевой аспект **audio**, то этот элемент представляет звуковой файл. Свойства ресурса **Audio** заполняются путем извлечения метаданных из такого файла.</span><span class="sxs-lookup"><span data-stu-id="4b562-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="4b562-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4b562-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4b562-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b562-108">Properties</span></span>

| <span data-ttu-id="4b562-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="4b562-109">Property name</span></span>         | <span data-ttu-id="4b562-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4b562-110">Type</span></span>    | <span data-ttu-id="4b562-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4b562-111">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="4b562-112">**album**</span><span class="sxs-lookup"><span data-stu-id="4b562-112">**album**</span></span>             | <span data-ttu-id="4b562-113">string</span><span class="sxs-lookup"><span data-stu-id="4b562-113">string</span></span>  | <span data-ttu-id="4b562-114">Название альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4b562-114">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="4b562-115">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="4b562-115">**albumArtist**</span></span>       | <span data-ttu-id="4b562-116">string</span><span class="sxs-lookup"><span data-stu-id="4b562-116">string</span></span>  | <span data-ttu-id="4b562-117">Название исполнителя альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4b562-117">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="4b562-118">**artist**</span><span class="sxs-lookup"><span data-stu-id="4b562-118">**artist**</span></span>            | <span data-ttu-id="4b562-119">string</span><span class="sxs-lookup"><span data-stu-id="4b562-119">string</span></span>  | <span data-ttu-id="4b562-120">Исполнитель для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4b562-120">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="4b562-121">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="4b562-121">**bitrate**</span></span>           | <span data-ttu-id="4b562-122">Int32</span><span class="sxs-lookup"><span data-stu-id="4b562-122">Int32</span></span>   | <span data-ttu-id="4b562-123">Скорость передачи данных в кбит/с.</span><span class="sxs-lookup"><span data-stu-id="4b562-123">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="4b562-124">**composers**</span><span class="sxs-lookup"><span data-stu-id="4b562-124">**composers**</span></span>         | <span data-ttu-id="4b562-125">string</span><span class="sxs-lookup"><span data-stu-id="4b562-125">string</span></span>  | <span data-ttu-id="4b562-126">Имя композитора для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4b562-126">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="4b562-127">**copyright**</span><span class="sxs-lookup"><span data-stu-id="4b562-127">**copyright**</span></span>         | <span data-ttu-id="4b562-128">string</span><span class="sxs-lookup"><span data-stu-id="4b562-128">string</span></span>  | <span data-ttu-id="4b562-129">Сведения об авторском праве для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4b562-129">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="4b562-130">**disc**</span><span class="sxs-lookup"><span data-stu-id="4b562-130">**disc**</span></span>              | <span data-ttu-id="4b562-131">Int32</span><span class="sxs-lookup"><span data-stu-id="4b562-131">Int32</span></span>   | <span data-ttu-id="4b562-132">Номер диска, с которого был взят этот звуковой файл.</span><span class="sxs-lookup"><span data-stu-id="4b562-132">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="4b562-133">**discCount**</span><span class="sxs-lookup"><span data-stu-id="4b562-133">**discCount**</span></span>         | <span data-ttu-id="4b562-134">Int32</span><span class="sxs-lookup"><span data-stu-id="4b562-134">Int32</span></span>   | <span data-ttu-id="4b562-135">Общее количество дисков для этого альбома.</span><span class="sxs-lookup"><span data-stu-id="4b562-135">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="4b562-136">**duration**</span><span class="sxs-lookup"><span data-stu-id="4b562-136">**duration**</span></span>          | <span data-ttu-id="4b562-137">Int64</span><span class="sxs-lookup"><span data-stu-id="4b562-137">Int64</span></span>   | <span data-ttu-id="4b562-138">Длительность воспроизведения звукового файла в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="4b562-138">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="4b562-139">**genre**</span><span class="sxs-lookup"><span data-stu-id="4b562-139">**genre**</span></span>             | <span data-ttu-id="4b562-140">string</span><span class="sxs-lookup"><span data-stu-id="4b562-140">string</span></span>  | <span data-ttu-id="4b562-141">Жанр этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4b562-141">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="4b562-142">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="4b562-142">**hasDrm**</span></span>            | <span data-ttu-id="4b562-143">boolean</span><span class="sxs-lookup"><span data-stu-id="4b562-143">boolean</span></span> | <span data-ttu-id="4b562-144">Указывает, защищен ли файл с помощью технологии управления цифровыми правами.</span><span class="sxs-lookup"><span data-stu-id="4b562-144">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="4b562-145">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="4b562-145">**isVariableBitrate**</span></span> | <span data-ttu-id="4b562-146">boolean</span><span class="sxs-lookup"><span data-stu-id="4b562-146">boolean</span></span> | <span data-ttu-id="4b562-147">Указывает, закодирован ли файл с использованием переменной скорости передачи данных.</span><span class="sxs-lookup"><span data-stu-id="4b562-147">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="4b562-148">**title**</span><span class="sxs-lookup"><span data-stu-id="4b562-148">**title**</span></span>             | <span data-ttu-id="4b562-149">строка</span><span class="sxs-lookup"><span data-stu-id="4b562-149">string</span></span>  | <span data-ttu-id="4b562-150">Название звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4b562-150">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="4b562-151">**track**</span><span class="sxs-lookup"><span data-stu-id="4b562-151">**track**</span></span>             | <span data-ttu-id="4b562-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4b562-152">Int32</span></span>   | <span data-ttu-id="4b562-153">Номер дорожки на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4b562-153">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="4b562-154">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="4b562-154">**trackCount**</span></span>        | <span data-ttu-id="4b562-155">Int32</span><span class="sxs-lookup"><span data-stu-id="4b562-155">Int32</span></span>   | <span data-ttu-id="4b562-156">Общее количество дорожек на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4b562-156">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="4b562-157">**year**</span><span class="sxs-lookup"><span data-stu-id="4b562-157">**year**</span></span>              | <span data-ttu-id="4b562-158">Int32</span><span class="sxs-lookup"><span data-stu-id="4b562-158">Int32</span></span>   | <span data-ttu-id="4b562-159">Год записи звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4b562-159">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="4b562-160">Примечания</span><span class="sxs-lookup"><span data-stu-id="4b562-160">Remarks</span></span>

<span data-ttu-id="4b562-161">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="4b562-161">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
