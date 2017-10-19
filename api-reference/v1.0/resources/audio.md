---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Audio
ms.openlocfilehash: 43b9999ecfb472a82e00a12ca820fdf8548eec64
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="audio-facet"></a><span data-ttu-id="89c89-102">Аспект Audio</span><span class="sxs-lookup"><span data-stu-id="89c89-102">Audio facet</span></span>

<span data-ttu-id="89c89-103">Ресурс **Audio** группирует свойства элемента, связанные со звуком, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="89c89-103">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="89c89-104">Если у элемента [**DriveItem**](driveitem.md) есть аспект **audio**, значение которого не равно null, то этот элемент представляет звуковой файл.</span><span class="sxs-lookup"><span data-stu-id="89c89-104">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the Audio resource are populated by extracting metadata from the file.</span></span>
<span data-ttu-id="89c89-105">Свойства ресурса **Audio** заполняются путем извлечения метаданных из этого файла.</span><span class="sxs-lookup"><span data-stu-id="89c89-105">If a DriveItem has a non-null audio facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="89c89-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="89c89-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="89c89-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="89c89-107">Properties</span></span>

| <span data-ttu-id="89c89-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="89c89-108">Property name</span></span>         | <span data-ttu-id="89c89-109">Тип</span><span class="sxs-lookup"><span data-stu-id="89c89-109">Type</span></span>    | <span data-ttu-id="89c89-110">Описание</span><span class="sxs-lookup"><span data-stu-id="89c89-110">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="89c89-111">**album**</span><span class="sxs-lookup"><span data-stu-id="89c89-111">**album**</span></span>             | <span data-ttu-id="89c89-112">строка</span><span class="sxs-lookup"><span data-stu-id="89c89-112">string</span></span>  | <span data-ttu-id="89c89-113">Название альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="89c89-113">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="89c89-114">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="89c89-114">**albumArtist**</span></span>       | <span data-ttu-id="89c89-115">строка</span><span class="sxs-lookup"><span data-stu-id="89c89-115">string</span></span>  | <span data-ttu-id="89c89-116">Название исполнителя альбома для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="89c89-116">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="89c89-117">**artist**</span><span class="sxs-lookup"><span data-stu-id="89c89-117">**artist**</span></span>            | <span data-ttu-id="89c89-118">строка</span><span class="sxs-lookup"><span data-stu-id="89c89-118">string</span></span>  | <span data-ttu-id="89c89-119">Исполнитель для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="89c89-119">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="89c89-120">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="89c89-120">**bitrate**</span></span>           | <span data-ttu-id="89c89-121">Int32</span><span class="sxs-lookup"><span data-stu-id="89c89-121">Int32</span></span>   | <span data-ttu-id="89c89-122">Скорость передачи данных в кбит/с.</span><span class="sxs-lookup"><span data-stu-id="89c89-122">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="89c89-123">**composers**</span><span class="sxs-lookup"><span data-stu-id="89c89-123">**composers**</span></span>         | <span data-ttu-id="89c89-124">строка</span><span class="sxs-lookup"><span data-stu-id="89c89-124">string</span></span>  | <span data-ttu-id="89c89-125">Имя композитора для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="89c89-125">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="89c89-126">**copyright**</span><span class="sxs-lookup"><span data-stu-id="89c89-126">**copyright**</span></span>         | <span data-ttu-id="89c89-127">строка</span><span class="sxs-lookup"><span data-stu-id="89c89-127">string</span></span>  | <span data-ttu-id="89c89-128">Сведения об авторском праве для звукового файла.</span><span class="sxs-lookup"><span data-stu-id="89c89-128">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="89c89-129">**disc**</span><span class="sxs-lookup"><span data-stu-id="89c89-129">**disc**</span></span>              | <span data-ttu-id="89c89-130">Int32</span><span class="sxs-lookup"><span data-stu-id="89c89-130">Int32</span></span>   | <span data-ttu-id="89c89-131">Номер диска, с которого был взят этот звуковой файл.</span><span class="sxs-lookup"><span data-stu-id="89c89-131">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="89c89-132">**discCount**</span><span class="sxs-lookup"><span data-stu-id="89c89-132">**discCount**</span></span>         | <span data-ttu-id="89c89-133">Int32</span><span class="sxs-lookup"><span data-stu-id="89c89-133">Int32</span></span>   | <span data-ttu-id="89c89-134">Общее количество дисков для этого альбома.</span><span class="sxs-lookup"><span data-stu-id="89c89-134">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="89c89-135">**duration**</span><span class="sxs-lookup"><span data-stu-id="89c89-135">**duration**</span></span>          | <span data-ttu-id="89c89-136">Int64</span><span class="sxs-lookup"><span data-stu-id="89c89-136">Int64</span></span>   | <span data-ttu-id="89c89-137">Длительность воспроизведения звукового файла в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="89c89-137">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="89c89-138">**genre**</span><span class="sxs-lookup"><span data-stu-id="89c89-138">**genre**</span></span>             | <span data-ttu-id="89c89-139">строка</span><span class="sxs-lookup"><span data-stu-id="89c89-139">string</span></span>  | <span data-ttu-id="89c89-140">Жанр этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="89c89-140">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="89c89-141">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="89c89-141">**hasDrm**</span></span>            | <span data-ttu-id="89c89-142">boolean</span><span class="sxs-lookup"><span data-stu-id="89c89-142">boolean</span></span> | <span data-ttu-id="89c89-143">Указывает, защищен ли файл с помощью технологии управления цифровыми правами.</span><span class="sxs-lookup"><span data-stu-id="89c89-143">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="89c89-144">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="89c89-144">**isVariableBitrate**</span></span> | <span data-ttu-id="89c89-145">boolean</span><span class="sxs-lookup"><span data-stu-id="89c89-145">boolean</span></span> | <span data-ttu-id="89c89-146">Указывает, закодирован ли файл с использованием переменной скорости передачи данных.</span><span class="sxs-lookup"><span data-stu-id="89c89-146">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="89c89-147">**title**</span><span class="sxs-lookup"><span data-stu-id="89c89-147">**title**</span></span>             | <span data-ttu-id="89c89-148">строка</span><span class="sxs-lookup"><span data-stu-id="89c89-148">string</span></span>  | <span data-ttu-id="89c89-149">Название звукового файла.</span><span class="sxs-lookup"><span data-stu-id="89c89-149">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="89c89-150">**track**</span><span class="sxs-lookup"><span data-stu-id="89c89-150">**track**</span></span>             | <span data-ttu-id="89c89-151">Int32</span><span class="sxs-lookup"><span data-stu-id="89c89-151">Int32</span></span>   | <span data-ttu-id="89c89-152">Номер дорожки на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="89c89-152">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="89c89-153">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="89c89-153">**trackCount**</span></span>        | <span data-ttu-id="89c89-154">Int32</span><span class="sxs-lookup"><span data-stu-id="89c89-154">Int32</span></span>   | <span data-ttu-id="89c89-155">Общее количество дорожек на исходном диске для этого звукового файла.</span><span class="sxs-lookup"><span data-stu-id="89c89-155">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="89c89-156">**year**</span><span class="sxs-lookup"><span data-stu-id="89c89-156">**year**</span></span>              | <span data-ttu-id="89c89-157">Int32</span><span class="sxs-lookup"><span data-stu-id="89c89-157">Int32</span></span>   | <span data-ttu-id="89c89-158">Год записи звукового файла.</span><span class="sxs-lookup"><span data-stu-id="89c89-158">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="89c89-159">Примечания</span><span class="sxs-lookup"><span data-stu-id="89c89-159">Remarks</span></span>

<span data-ttu-id="89c89-160">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="89c89-160">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
