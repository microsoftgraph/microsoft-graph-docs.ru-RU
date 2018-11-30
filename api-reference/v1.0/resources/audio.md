---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Audio
ms.openlocfilehash: e68b70565f0eccd7847fba2b8085661071a75ae7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025548"
---
# <a name="audio-facet"></a><span data-ttu-id="bfa44-102">Аспект Audio</span><span class="sxs-lookup"><span data-stu-id="bfa44-102">Audio facet</span></span>

<span data-ttu-id="bfa44-103">Ресурс **Audio** группирует свойства элемента, связанные со звуком, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="bfa44-103">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="bfa44-p101">Если у элемента [**DriveItem**](driveitem.md) есть ненулевой аспект **audio**, то этот элемент представляет звуковой файл. Свойства ресурса **Audio** заполняются путем извлечения метаданных из такого файла.</span><span class="sxs-lookup"><span data-stu-id="bfa44-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="bfa44-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bfa44-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="bfa44-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bfa44-107">Properties</span></span>

| <span data-ttu-id="bfa44-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="bfa44-108">Property name</span></span>         | <span data-ttu-id="bfa44-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bfa44-109">Type</span></span>    | <span data-ttu-id="bfa44-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bfa44-110">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="bfa44-111">**album**</span><span class="sxs-lookup"><span data-stu-id="bfa44-111">**album**</span></span>             | <span data-ttu-id="bfa44-112">строка</span><span class="sxs-lookup"><span data-stu-id="bfa44-112">string</span></span>  | <span data-ttu-id="bfa44-113">Название альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="bfa44-113">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="bfa44-114">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="bfa44-114">**albumArtist**</span></span>       | <span data-ttu-id="bfa44-115">строка</span><span class="sxs-lookup"><span data-stu-id="bfa44-115">string</span></span>  | <span data-ttu-id="bfa44-116">Название исполнителя альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="bfa44-116">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="bfa44-117">**artist**</span><span class="sxs-lookup"><span data-stu-id="bfa44-117">**artist**</span></span>            | <span data-ttu-id="bfa44-118">строка</span><span class="sxs-lookup"><span data-stu-id="bfa44-118">string</span></span>  | <span data-ttu-id="bfa44-119">Исполнитель для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="bfa44-119">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="bfa44-120">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="bfa44-120">**bitrate**</span></span>           | <span data-ttu-id="bfa44-121">Int64</span><span class="sxs-lookup"><span data-stu-id="bfa44-121">Int64</span></span>   | <span data-ttu-id="bfa44-122">Скорость передачи данных в кбит/с.</span><span class="sxs-lookup"><span data-stu-id="bfa44-122">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="bfa44-123">**composers**</span><span class="sxs-lookup"><span data-stu-id="bfa44-123">**composers**</span></span>         | <span data-ttu-id="bfa44-124">строка</span><span class="sxs-lookup"><span data-stu-id="bfa44-124">string</span></span>  | <span data-ttu-id="bfa44-125">Имя композитора для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="bfa44-125">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="bfa44-126">**copyright**</span><span class="sxs-lookup"><span data-stu-id="bfa44-126">**copyright**</span></span>         | <span data-ttu-id="bfa44-127">строка</span><span class="sxs-lookup"><span data-stu-id="bfa44-127">string</span></span>  | <span data-ttu-id="bfa44-128">Сведения об авторском праве для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="bfa44-128">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="bfa44-129">**disc**</span><span class="sxs-lookup"><span data-stu-id="bfa44-129">**disc**</span></span>              | <span data-ttu-id="bfa44-130">Int16</span><span class="sxs-lookup"><span data-stu-id="bfa44-130">Int16</span></span>   | <span data-ttu-id="bfa44-131">Номер диска, с которого был взят этот звуковой файл.</span><span class="sxs-lookup"><span data-stu-id="bfa44-131">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="bfa44-132">**discCount**</span><span class="sxs-lookup"><span data-stu-id="bfa44-132">**discCount**</span></span>         | <span data-ttu-id="bfa44-133">Int16</span><span class="sxs-lookup"><span data-stu-id="bfa44-133">Int16</span></span>   | <span data-ttu-id="bfa44-134">Общее количество дисков для этого альбома.</span><span class="sxs-lookup"><span data-stu-id="bfa44-134">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="bfa44-135">**duration**</span><span class="sxs-lookup"><span data-stu-id="bfa44-135">**duration**</span></span>          | <span data-ttu-id="bfa44-136">Int64</span><span class="sxs-lookup"><span data-stu-id="bfa44-136">Int64</span></span>   | <span data-ttu-id="bfa44-137">Длительность воспроизведения звукового файла в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="bfa44-137">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="bfa44-138">**genre**</span><span class="sxs-lookup"><span data-stu-id="bfa44-138">**genre**</span></span>             | <span data-ttu-id="bfa44-139">строка</span><span class="sxs-lookup"><span data-stu-id="bfa44-139">string</span></span>  | <span data-ttu-id="bfa44-140">Жанр этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="bfa44-140">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="bfa44-141">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="bfa44-141">**hasDrm**</span></span>            | <span data-ttu-id="bfa44-142">boolean</span><span class="sxs-lookup"><span data-stu-id="bfa44-142">boolean</span></span> | <span data-ttu-id="bfa44-143">Указывает, защищен ли файл с помощью технологии управления цифровыми правами.</span><span class="sxs-lookup"><span data-stu-id="bfa44-143">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="bfa44-144">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="bfa44-144">**isVariableBitrate**</span></span> | <span data-ttu-id="bfa44-145">boolean</span><span class="sxs-lookup"><span data-stu-id="bfa44-145">boolean</span></span> | <span data-ttu-id="bfa44-146">Указывает, закодирован ли файл с использованием переменной скорости передачи данных.</span><span class="sxs-lookup"><span data-stu-id="bfa44-146">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="bfa44-147">**title**</span><span class="sxs-lookup"><span data-stu-id="bfa44-147">**title**</span></span>             | <span data-ttu-id="bfa44-148">строка</span><span class="sxs-lookup"><span data-stu-id="bfa44-148">string</span></span>  | <span data-ttu-id="bfa44-149">Название звукового файла.</span><span class="sxs-lookup"><span data-stu-id="bfa44-149">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="bfa44-150">**track**</span><span class="sxs-lookup"><span data-stu-id="bfa44-150">**track**</span></span>             | <span data-ttu-id="bfa44-151">Int32</span><span class="sxs-lookup"><span data-stu-id="bfa44-151">Int32</span></span>   | <span data-ttu-id="bfa44-152">Номер дорожки на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="bfa44-152">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="bfa44-153">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="bfa44-153">**trackCount**</span></span>        | <span data-ttu-id="bfa44-154">Int32</span><span class="sxs-lookup"><span data-stu-id="bfa44-154">Int32</span></span>   | <span data-ttu-id="bfa44-155">Общее количество дорожек на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="bfa44-155">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="bfa44-156">**year**</span><span class="sxs-lookup"><span data-stu-id="bfa44-156">**year**</span></span>              | <span data-ttu-id="bfa44-157">Int32</span><span class="sxs-lookup"><span data-stu-id="bfa44-157">Int32</span></span>   | <span data-ttu-id="bfa44-158">Год записи звукового файла.</span><span class="sxs-lookup"><span data-stu-id="bfa44-158">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="bfa44-159">Примечания</span><span class="sxs-lookup"><span data-stu-id="bfa44-159">Remarks</span></span>

<span data-ttu-id="bfa44-160">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="bfa44-160">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
