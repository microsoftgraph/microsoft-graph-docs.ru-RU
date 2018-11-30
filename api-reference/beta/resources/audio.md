---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Audio
ms.openlocfilehash: 1472bffec12ed5626a65ea71b971dc5bc2b77aa9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076745"
---
# <a name="audio-facet"></a><span data-ttu-id="05d10-102">Аспект Audio</span><span class="sxs-lookup"><span data-stu-id="05d10-102">Audio facet</span></span>

> <span data-ttu-id="05d10-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="05d10-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05d10-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05d10-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="05d10-105">Ресурс **Audio** группирует свойства элемента, связанные со звуком, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="05d10-105">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="05d10-p102">Если у элемента [**DriveItem**](driveitem.md) есть ненулевой аспект **audio**, то этот элемент представляет звуковой файл. Свойства ресурса **Audio** заполняются путем извлечения метаданных из такого файла.</span><span class="sxs-lookup"><span data-stu-id="05d10-p102">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="05d10-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05d10-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="05d10-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="05d10-109">Properties</span></span>

| <span data-ttu-id="05d10-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="05d10-110">Property name</span></span>         | <span data-ttu-id="05d10-111">Тип</span><span class="sxs-lookup"><span data-stu-id="05d10-111">Type</span></span>    | <span data-ttu-id="05d10-112">Описание</span><span class="sxs-lookup"><span data-stu-id="05d10-112">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="05d10-113">**album**</span><span class="sxs-lookup"><span data-stu-id="05d10-113">**album**</span></span>             | <span data-ttu-id="05d10-114">строка</span><span class="sxs-lookup"><span data-stu-id="05d10-114">string</span></span>  | <span data-ttu-id="05d10-115">Название альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="05d10-115">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="05d10-116">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="05d10-116">**albumArtist**</span></span>       | <span data-ttu-id="05d10-117">строка</span><span class="sxs-lookup"><span data-stu-id="05d10-117">string</span></span>  | <span data-ttu-id="05d10-118">Название исполнителя альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="05d10-118">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="05d10-119">**artist**</span><span class="sxs-lookup"><span data-stu-id="05d10-119">**artist**</span></span>            | <span data-ttu-id="05d10-120">строка</span><span class="sxs-lookup"><span data-stu-id="05d10-120">string</span></span>  | <span data-ttu-id="05d10-121">Исполнитель для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="05d10-121">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="05d10-122">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="05d10-122">**bitrate**</span></span>           | <span data-ttu-id="05d10-123">Int32</span><span class="sxs-lookup"><span data-stu-id="05d10-123">Int32</span></span>   | <span data-ttu-id="05d10-124">Скорость передачи данных в кбит/с.</span><span class="sxs-lookup"><span data-stu-id="05d10-124">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="05d10-125">**composers**</span><span class="sxs-lookup"><span data-stu-id="05d10-125">**composers**</span></span>         | <span data-ttu-id="05d10-126">строка</span><span class="sxs-lookup"><span data-stu-id="05d10-126">string</span></span>  | <span data-ttu-id="05d10-127">Имя композитора для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="05d10-127">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="05d10-128">**copyright**</span><span class="sxs-lookup"><span data-stu-id="05d10-128">**copyright**</span></span>         | <span data-ttu-id="05d10-129">строка</span><span class="sxs-lookup"><span data-stu-id="05d10-129">string</span></span>  | <span data-ttu-id="05d10-130">Сведения об авторском праве для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="05d10-130">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="05d10-131">**disc**</span><span class="sxs-lookup"><span data-stu-id="05d10-131">**disc**</span></span>              | <span data-ttu-id="05d10-132">Int32</span><span class="sxs-lookup"><span data-stu-id="05d10-132">Int32</span></span>   | <span data-ttu-id="05d10-133">Номер диска, с которого был взят этот звуковой файл.</span><span class="sxs-lookup"><span data-stu-id="05d10-133">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="05d10-134">**discCount**</span><span class="sxs-lookup"><span data-stu-id="05d10-134">**discCount**</span></span>         | <span data-ttu-id="05d10-135">Int32</span><span class="sxs-lookup"><span data-stu-id="05d10-135">Int32</span></span>   | <span data-ttu-id="05d10-136">Общее количество дисков для этого альбома.</span><span class="sxs-lookup"><span data-stu-id="05d10-136">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="05d10-137">**duration**</span><span class="sxs-lookup"><span data-stu-id="05d10-137">**duration**</span></span>          | <span data-ttu-id="05d10-138">Int64</span><span class="sxs-lookup"><span data-stu-id="05d10-138">Int64</span></span>   | <span data-ttu-id="05d10-139">Длительность воспроизведения звукового файла в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="05d10-139">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="05d10-140">**genre**</span><span class="sxs-lookup"><span data-stu-id="05d10-140">**genre**</span></span>             | <span data-ttu-id="05d10-141">строка</span><span class="sxs-lookup"><span data-stu-id="05d10-141">string</span></span>  | <span data-ttu-id="05d10-142">Жанр этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="05d10-142">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="05d10-143">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="05d10-143">**hasDrm**</span></span>            | <span data-ttu-id="05d10-144">boolean</span><span class="sxs-lookup"><span data-stu-id="05d10-144">boolean</span></span> | <span data-ttu-id="05d10-145">Указывает, защищен ли файл с помощью технологии управления цифровыми правами.</span><span class="sxs-lookup"><span data-stu-id="05d10-145">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="05d10-146">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="05d10-146">**isVariableBitrate**</span></span> | <span data-ttu-id="05d10-147">boolean</span><span class="sxs-lookup"><span data-stu-id="05d10-147">boolean</span></span> | <span data-ttu-id="05d10-148">Указывает, закодирован ли файл с использованием переменной скорости передачи данных.</span><span class="sxs-lookup"><span data-stu-id="05d10-148">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="05d10-149">**title**</span><span class="sxs-lookup"><span data-stu-id="05d10-149">**title**</span></span>             | <span data-ttu-id="05d10-150">строка</span><span class="sxs-lookup"><span data-stu-id="05d10-150">string</span></span>  | <span data-ttu-id="05d10-151">Название звукового файла.</span><span class="sxs-lookup"><span data-stu-id="05d10-151">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="05d10-152">**track**</span><span class="sxs-lookup"><span data-stu-id="05d10-152">**track**</span></span>             | <span data-ttu-id="05d10-153">Int32</span><span class="sxs-lookup"><span data-stu-id="05d10-153">Int32</span></span>   | <span data-ttu-id="05d10-154">Номер дорожки на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="05d10-154">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="05d10-155">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="05d10-155">**trackCount**</span></span>        | <span data-ttu-id="05d10-156">Int32</span><span class="sxs-lookup"><span data-stu-id="05d10-156">Int32</span></span>   | <span data-ttu-id="05d10-157">Общее количество дорожек на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="05d10-157">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="05d10-158">**year**</span><span class="sxs-lookup"><span data-stu-id="05d10-158">**year**</span></span>              | <span data-ttu-id="05d10-159">Int32</span><span class="sxs-lookup"><span data-stu-id="05d10-159">Int32</span></span>   | <span data-ttu-id="05d10-160">Год записи звукового файла.</span><span class="sxs-lookup"><span data-stu-id="05d10-160">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="05d10-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="05d10-161">Remarks</span></span>

<span data-ttu-id="05d10-162">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="05d10-162">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
