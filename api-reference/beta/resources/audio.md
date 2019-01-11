---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Audio
localization_priority: Normal
ms.openlocfilehash: ead665ee4977a563ebb6b24636b627d72a2428dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871591"
---
# <a name="audio-facet"></a><span data-ttu-id="4ff87-102">Аспект Audio</span><span class="sxs-lookup"><span data-stu-id="4ff87-102">Audio facet</span></span>

> <span data-ttu-id="4ff87-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4ff87-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ff87-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ff87-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ff87-105">Ресурс **Audio** группирует свойства элемента, связанные со звуком, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="4ff87-105">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="4ff87-p102">Если у элемента [**DriveItem**](driveitem.md) есть ненулевой аспект **audio**, то этот элемент представляет звуковой файл. Свойства ресурса **Audio** заполняются путем извлечения метаданных из такого файла.</span><span class="sxs-lookup"><span data-stu-id="4ff87-p102">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="4ff87-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ff87-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4ff87-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ff87-109">Properties</span></span>

| <span data-ttu-id="4ff87-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="4ff87-110">Property name</span></span>         | <span data-ttu-id="4ff87-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4ff87-111">Type</span></span>    | <span data-ttu-id="4ff87-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4ff87-112">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="4ff87-113">**album**</span><span class="sxs-lookup"><span data-stu-id="4ff87-113">**album**</span></span>             | <span data-ttu-id="4ff87-114">строка</span><span class="sxs-lookup"><span data-stu-id="4ff87-114">string</span></span>  | <span data-ttu-id="4ff87-115">Название альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4ff87-115">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="4ff87-116">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="4ff87-116">**albumArtist**</span></span>       | <span data-ttu-id="4ff87-117">строка</span><span class="sxs-lookup"><span data-stu-id="4ff87-117">string</span></span>  | <span data-ttu-id="4ff87-118">Название исполнителя альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4ff87-118">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="4ff87-119">**artist**</span><span class="sxs-lookup"><span data-stu-id="4ff87-119">**artist**</span></span>            | <span data-ttu-id="4ff87-120">строка</span><span class="sxs-lookup"><span data-stu-id="4ff87-120">string</span></span>  | <span data-ttu-id="4ff87-121">Исполнитель для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4ff87-121">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="4ff87-122">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="4ff87-122">**bitrate**</span></span>           | <span data-ttu-id="4ff87-123">Int32</span><span class="sxs-lookup"><span data-stu-id="4ff87-123">Int32</span></span>   | <span data-ttu-id="4ff87-124">Скорость передачи данных в кбит/с.</span><span class="sxs-lookup"><span data-stu-id="4ff87-124">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="4ff87-125">**composers**</span><span class="sxs-lookup"><span data-stu-id="4ff87-125">**composers**</span></span>         | <span data-ttu-id="4ff87-126">строка</span><span class="sxs-lookup"><span data-stu-id="4ff87-126">string</span></span>  | <span data-ttu-id="4ff87-127">Имя композитора для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4ff87-127">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="4ff87-128">**copyright**</span><span class="sxs-lookup"><span data-stu-id="4ff87-128">**copyright**</span></span>         | <span data-ttu-id="4ff87-129">строка</span><span class="sxs-lookup"><span data-stu-id="4ff87-129">string</span></span>  | <span data-ttu-id="4ff87-130">Сведения об авторском праве для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4ff87-130">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="4ff87-131">**disc**</span><span class="sxs-lookup"><span data-stu-id="4ff87-131">**disc**</span></span>              | <span data-ttu-id="4ff87-132">Int32</span><span class="sxs-lookup"><span data-stu-id="4ff87-132">Int32</span></span>   | <span data-ttu-id="4ff87-133">Номер диска, с которого был взят этот звуковой файл.</span><span class="sxs-lookup"><span data-stu-id="4ff87-133">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="4ff87-134">**discCount**</span><span class="sxs-lookup"><span data-stu-id="4ff87-134">**discCount**</span></span>         | <span data-ttu-id="4ff87-135">Int32</span><span class="sxs-lookup"><span data-stu-id="4ff87-135">Int32</span></span>   | <span data-ttu-id="4ff87-136">Общее количество дисков для этого альбома.</span><span class="sxs-lookup"><span data-stu-id="4ff87-136">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="4ff87-137">**duration**</span><span class="sxs-lookup"><span data-stu-id="4ff87-137">**duration**</span></span>          | <span data-ttu-id="4ff87-138">Int64</span><span class="sxs-lookup"><span data-stu-id="4ff87-138">Int64</span></span>   | <span data-ttu-id="4ff87-139">Длительность воспроизведения звукового файла в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="4ff87-139">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="4ff87-140">**genre**</span><span class="sxs-lookup"><span data-stu-id="4ff87-140">**genre**</span></span>             | <span data-ttu-id="4ff87-141">строка</span><span class="sxs-lookup"><span data-stu-id="4ff87-141">string</span></span>  | <span data-ttu-id="4ff87-142">Жанр этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4ff87-142">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="4ff87-143">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="4ff87-143">**hasDrm**</span></span>            | <span data-ttu-id="4ff87-144">boolean</span><span class="sxs-lookup"><span data-stu-id="4ff87-144">boolean</span></span> | <span data-ttu-id="4ff87-145">Указывает, защищен ли файл с помощью технологии управления цифровыми правами.</span><span class="sxs-lookup"><span data-stu-id="4ff87-145">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="4ff87-146">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="4ff87-146">**isVariableBitrate**</span></span> | <span data-ttu-id="4ff87-147">boolean</span><span class="sxs-lookup"><span data-stu-id="4ff87-147">boolean</span></span> | <span data-ttu-id="4ff87-148">Указывает, закодирован ли файл с использованием переменной скорости передачи данных.</span><span class="sxs-lookup"><span data-stu-id="4ff87-148">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="4ff87-149">**title**</span><span class="sxs-lookup"><span data-stu-id="4ff87-149">**title**</span></span>             | <span data-ttu-id="4ff87-150">строка</span><span class="sxs-lookup"><span data-stu-id="4ff87-150">string</span></span>  | <span data-ttu-id="4ff87-151">Название звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4ff87-151">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="4ff87-152">**track**</span><span class="sxs-lookup"><span data-stu-id="4ff87-152">**track**</span></span>             | <span data-ttu-id="4ff87-153">Int32</span><span class="sxs-lookup"><span data-stu-id="4ff87-153">Int32</span></span>   | <span data-ttu-id="4ff87-154">Номер дорожки на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4ff87-154">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="4ff87-155">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="4ff87-155">**trackCount**</span></span>        | <span data-ttu-id="4ff87-156">Int32</span><span class="sxs-lookup"><span data-stu-id="4ff87-156">Int32</span></span>   | <span data-ttu-id="4ff87-157">Общее количество дорожек на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4ff87-157">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="4ff87-158">**year**</span><span class="sxs-lookup"><span data-stu-id="4ff87-158">**year**</span></span>              | <span data-ttu-id="4ff87-159">Int32</span><span class="sxs-lookup"><span data-stu-id="4ff87-159">Int32</span></span>   | <span data-ttu-id="4ff87-160">Год записи звукового файла.</span><span class="sxs-lookup"><span data-stu-id="4ff87-160">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="4ff87-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="4ff87-161">Remarks</span></span>

<span data-ttu-id="4ff87-162">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="4ff87-162">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
