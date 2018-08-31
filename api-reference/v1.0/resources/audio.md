---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Звук
ms.openlocfilehash: e68b70565f0eccd7847fba2b8085661071a75ae7
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266235"
---
# <a name="audio-facet"></a><span data-ttu-id="f5076-102">Аспект Audio</span><span class="sxs-lookup"><span data-stu-id="f5076-102">Audio facet</span></span>

<span data-ttu-id="f5076-103">Ресурс **Звук** группирует свойства элемента, связанные со звуком, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="f5076-103">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="f5076-p101">Если у элемента [**DriveItem**](driveitem.md) есть ненулевой аспект **audio**, то этот элемент представляет звуковой файл. Свойства ресурса **Audio** заполняются путем извлечения метаданных из такого файла.</span><span class="sxs-lookup"><span data-stu-id="f5076-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="f5076-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5076-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f5076-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5076-107">Properties</span></span>

| <span data-ttu-id="f5076-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="f5076-108">Property name</span></span>         | <span data-ttu-id="f5076-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f5076-109">Type</span></span>    | <span data-ttu-id="f5076-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f5076-110">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="f5076-111">**альбом**</span><span class="sxs-lookup"><span data-stu-id="f5076-111">**album**</span></span>             | <span data-ttu-id="f5076-112">строка</span><span class="sxs-lookup"><span data-stu-id="f5076-112">string</span></span>  | <span data-ttu-id="f5076-113">Название альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="f5076-113">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="f5076-114">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="f5076-114">**albumArtist**</span></span>       | <span data-ttu-id="f5076-115">строка</span><span class="sxs-lookup"><span data-stu-id="f5076-115">string</span></span>  | <span data-ttu-id="f5076-116">Название исполнителя альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="f5076-116">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="f5076-117">**исполнитель**</span><span class="sxs-lookup"><span data-stu-id="f5076-117">**artist**</span></span>            | <span data-ttu-id="f5076-118">строка</span><span class="sxs-lookup"><span data-stu-id="f5076-118">string</span></span>  | <span data-ttu-id="f5076-119">Исполнитель для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="f5076-119">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="f5076-120">**Скорость**</span><span class="sxs-lookup"><span data-stu-id="f5076-120">**bitrate**</span></span>           | <span data-ttu-id="f5076-121">Int64</span><span class="sxs-lookup"><span data-stu-id="f5076-121">Int64</span></span>   | <span data-ttu-id="f5076-122">Скорость передачи данных в кбит/с.</span><span class="sxs-lookup"><span data-stu-id="f5076-122">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="f5076-123">**композиторы**</span><span class="sxs-lookup"><span data-stu-id="f5076-123">**composers**</span></span>         | <span data-ttu-id="f5076-124">строка</span><span class="sxs-lookup"><span data-stu-id="f5076-124">string</span></span>  | <span data-ttu-id="f5076-125">Имя композитора для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="f5076-125">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="f5076-126">**авторское право**</span><span class="sxs-lookup"><span data-stu-id="f5076-126">**copyright**</span></span>         | <span data-ttu-id="f5076-127">строка</span><span class="sxs-lookup"><span data-stu-id="f5076-127">string</span></span>  | <span data-ttu-id="f5076-128">Сведения об авторском праве для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="f5076-128">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="f5076-129">**диск**</span><span class="sxs-lookup"><span data-stu-id="f5076-129">**disc**</span></span>              | <span data-ttu-id="f5076-130">Int16</span><span class="sxs-lookup"><span data-stu-id="f5076-130">Int16</span></span>   | <span data-ttu-id="f5076-131">Номер диска, с которого был взят этот звуковой файл.</span><span class="sxs-lookup"><span data-stu-id="f5076-131">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="f5076-132">**discCount**</span><span class="sxs-lookup"><span data-stu-id="f5076-132">**discCount**</span></span>         | <span data-ttu-id="f5076-133">Int16</span><span class="sxs-lookup"><span data-stu-id="f5076-133">Int16</span></span>   | <span data-ttu-id="f5076-134">Общее количество дисков в этом альбоме.</span><span class="sxs-lookup"><span data-stu-id="f5076-134">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="f5076-135">**длительность**</span><span class="sxs-lookup"><span data-stu-id="f5076-135">**duration**</span></span>          | <span data-ttu-id="f5076-136">Int64</span><span class="sxs-lookup"><span data-stu-id="f5076-136">Int64</span></span>   | <span data-ttu-id="f5076-137">Длительность воспроизведения звукового файла в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="f5076-137">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="f5076-138">**жанр**</span><span class="sxs-lookup"><span data-stu-id="f5076-138">**genre**</span></span>             | <span data-ttu-id="f5076-139">строка</span><span class="sxs-lookup"><span data-stu-id="f5076-139">string</span></span>  | <span data-ttu-id="f5076-140">Жанр этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="f5076-140">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="f5076-141">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="f5076-141">**hasDrm**</span></span>            | <span data-ttu-id="f5076-142">логический</span><span class="sxs-lookup"><span data-stu-id="f5076-142">boolean</span></span> | <span data-ttu-id="f5076-143">Указывает, защищен ли файл с помощью технологии управления цифровыми правами.</span><span class="sxs-lookup"><span data-stu-id="f5076-143">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="f5076-144">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="f5076-144">**isVariableBitrate**</span></span> | <span data-ttu-id="f5076-145">логический</span><span class="sxs-lookup"><span data-stu-id="f5076-145">boolean</span></span> | <span data-ttu-id="f5076-146">Указывает, закодирован ли файл с использованием переменной скорости передачи данных.</span><span class="sxs-lookup"><span data-stu-id="f5076-146">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="f5076-147">**название**</span><span class="sxs-lookup"><span data-stu-id="f5076-147">**title**</span></span>             | <span data-ttu-id="f5076-148">строка</span><span class="sxs-lookup"><span data-stu-id="f5076-148">string</span></span>  | <span data-ttu-id="f5076-149">Название звукового файла.</span><span class="sxs-lookup"><span data-stu-id="f5076-149">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="f5076-150">**дорожка**</span><span class="sxs-lookup"><span data-stu-id="f5076-150">**track**</span></span>             | <span data-ttu-id="f5076-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f5076-151">Int32</span></span>   | <span data-ttu-id="f5076-152">Номер дорожки на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="f5076-152">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="f5076-153">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="f5076-153">**trackCount**</span></span>        | <span data-ttu-id="f5076-154">Int32</span><span class="sxs-lookup"><span data-stu-id="f5076-154">Int32</span></span>   | <span data-ttu-id="f5076-155">Общее количество дорожек на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="f5076-155">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="f5076-156">**год**</span><span class="sxs-lookup"><span data-stu-id="f5076-156">**year**</span></span>              | <span data-ttu-id="f5076-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f5076-157">Int32</span></span>   | <span data-ttu-id="f5076-158">Год записи звукового файла.</span><span class="sxs-lookup"><span data-stu-id="f5076-158">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="f5076-159">Примечания</span><span class="sxs-lookup"><span data-stu-id="f5076-159">Remarks</span></span>

<span data-ttu-id="f5076-160">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f5076-160">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
