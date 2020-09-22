---
author: JeremyKelley
description: Хеш-коды групп ресурсов, доступные в виде одной структуры для элемента.
ms.date: 09/10/2017
title: Hashes
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: df3629be679b714805ea6618b7aa963214f32793
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013610"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="2673e-103">Тип ресурса hashs</span><span class="sxs-lookup"><span data-stu-id="2673e-103">hashes resource type</span></span>

<span data-ttu-id="2673e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2673e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2673e-105">Группирует доступные хэши в единую структуру для элемента.</span><span class="sxs-lookup"><span data-stu-id="2673e-105">Groups available hashes into a single structure for an item.</span></span>

> [!NOTE]
> <span data-ttu-id="2673e-106">Не все службы предоставляют значение для всех перечисленных свойств хеша.</span><span class="sxs-lookup"><span data-stu-id="2673e-106">Not all services provide a value for all hash properties listed.</span></span> <span data-ttu-id="2673e-107">В OneDrive для бизнеса и SharePoint Server 2016, **sha1Hash**, **crc32Hash**и **sha256Hash** недоступны.</span><span class="sxs-lookup"><span data-stu-id="2673e-107">In OneDrive for Business and SharePoint Server 2016, **sha1Hash**, **crc32Hash**, and **sha256Hash** are not available.</span></span> <span data-ttu-id="2673e-108">В OneDrive персональный хэш **quickXorHash** недоступен.</span><span class="sxs-lookup"><span data-stu-id="2673e-108">In OneDrive Personal, **quickXorHash** is not available.</span></span>

## <a name="properties"></a><span data-ttu-id="2673e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2673e-109">Properties</span></span>

| <span data-ttu-id="2673e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2673e-110">Property</span></span>         | <span data-ttu-id="2673e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2673e-111">Type</span></span>   | <span data-ttu-id="2673e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2673e-112">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="2673e-113">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="2673e-113">**sha1Hash**</span></span>     | <span data-ttu-id="2673e-114">String</span><span class="sxs-lookup"><span data-stu-id="2673e-114">String</span></span> | <span data-ttu-id="2673e-p102">Хэш SHA1 для содержимого файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2673e-p102">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="2673e-117">**sha256Hash**</span><span class="sxs-lookup"><span data-stu-id="2673e-117">**sha256Hash**</span></span>   | <span data-ttu-id="2673e-118">String</span><span class="sxs-lookup"><span data-stu-id="2673e-118">String</span></span> | <span data-ttu-id="2673e-119">Хэш SHA256 для содержимого файла (если он доступен).</span><span class="sxs-lookup"><span data-stu-id="2673e-119">SHA256 hash for the contents of the file (if available).</span></span> <span data-ttu-id="2673e-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2673e-120">Read-only.</span></span> |
| <span data-ttu-id="2673e-121">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="2673e-121">**crc32Hash**</span></span>    | <span data-ttu-id="2673e-122">String</span><span class="sxs-lookup"><span data-stu-id="2673e-122">String</span></span> | <span data-ttu-id="2673e-p104">Значение CRC32 файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2673e-p104">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="2673e-125">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="2673e-125">**quickXorHash**</span></span> | <span data-ttu-id="2673e-126">Строка</span><span class="sxs-lookup"><span data-stu-id="2673e-126">String</span></span> | <span data-ttu-id="2673e-p105">Особый хэш файла, который можно использовать, чтобы определить, было ли изменено содержимое файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2673e-p105">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

> <span data-ttu-id="2673e-129">**Примечание:** В случаях, когда хэш-значения недоступны, значения хеша для элемента будут обновлены после загрузки элемента.</span><span class="sxs-lookup"><span data-stu-id="2673e-129">**Note:** In cases where the hash values are not available, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2673e-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2673e-130">JSON representation</span></span>

<span data-ttu-id="2673e-131">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2673e-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string (hex)",
  "sha1Hash": "string (hex)",
  "sha256Hash": "string (hex)",
  "quickXorHash": "string (base64)"
}
```

## <a name="see-also"></a><span data-ttu-id="2673e-132">См. также</span><span class="sxs-lookup"><span data-stu-id="2673e-132">See also</span></span>

- <span data-ttu-id="2673e-133">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="2673e-133">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
- <span data-ttu-id="2673e-134">Пример вычисления значения **quickXorHash** для файла см. в [фрагменте кода QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).</span><span class="sxs-lookup"><span data-stu-id="2673e-134">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes",
  "suppressions": []
}
-->


