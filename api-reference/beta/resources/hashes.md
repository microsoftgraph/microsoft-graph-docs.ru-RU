---
author: JeremyKelley
description: Хеш-коды групп ресурсов, доступные в виде одной структуры для элемента.
ms.date: 09/10/2017
title: Hashes
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 985efa857fdf9aaa254884e04bfccf1d780d5b8c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496931"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="ab3cb-103">Тип ресурса hashs</span><span class="sxs-lookup"><span data-stu-id="ab3cb-103">hashes resource type</span></span>

<span data-ttu-id="ab3cb-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ab3cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab3cb-105">Группирует доступные хэши в единую структуру для элемента.</span><span class="sxs-lookup"><span data-stu-id="ab3cb-105">Groups available hashes into a single structure for an item.</span></span>

> [!NOTE]
> <span data-ttu-id="ab3cb-106">Не все службы предоставляют значение для всех перечисленных свойств хеша.</span><span class="sxs-lookup"><span data-stu-id="ab3cb-106">Not all services provide a value for all hash properties listed.</span></span> <span data-ttu-id="ab3cb-107">В OneDrive для бизнеса и SharePoint Server 2016, **sha1Hash**, **crc32Hash**и **sha256Hash** недоступны.</span><span class="sxs-lookup"><span data-stu-id="ab3cb-107">In OneDrive for Business and SharePoint Server 2016, **sha1Hash**, **crc32Hash**, and **sha256Hash** are not available.</span></span> <span data-ttu-id="ab3cb-108">В OneDrive персональный хэш **quickXorHash** недоступен.</span><span class="sxs-lookup"><span data-stu-id="ab3cb-108">In OneDrive Personal, **quickXorHash** is not available.</span></span>

## <a name="properties"></a><span data-ttu-id="ab3cb-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab3cb-109">Properties</span></span>

| <span data-ttu-id="ab3cb-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab3cb-110">Property</span></span>         | <span data-ttu-id="ab3cb-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ab3cb-111">Type</span></span>   | <span data-ttu-id="ab3cb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ab3cb-112">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="ab3cb-113">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="ab3cb-113">**sha1Hash**</span></span>     | <span data-ttu-id="ab3cb-114">String</span><span class="sxs-lookup"><span data-stu-id="ab3cb-114">String</span></span> | <span data-ttu-id="ab3cb-p102">Хэш SHA1 для содержимого файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab3cb-p102">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="ab3cb-117">**sha256Hash**</span><span class="sxs-lookup"><span data-stu-id="ab3cb-117">**sha256Hash**</span></span>   | <span data-ttu-id="ab3cb-118">String</span><span class="sxs-lookup"><span data-stu-id="ab3cb-118">String</span></span> | <span data-ttu-id="ab3cb-119">Хэш SHA256 для содержимого файла (если он доступен).</span><span class="sxs-lookup"><span data-stu-id="ab3cb-119">SHA256 hash for the contents of the file (if available).</span></span> <span data-ttu-id="ab3cb-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab3cb-120">Read-only.</span></span> |
| <span data-ttu-id="ab3cb-121">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="ab3cb-121">**crc32Hash**</span></span>    | <span data-ttu-id="ab3cb-122">String</span><span class="sxs-lookup"><span data-stu-id="ab3cb-122">String</span></span> | <span data-ttu-id="ab3cb-p104">Значение CRC32 файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab3cb-p104">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="ab3cb-125">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="ab3cb-125">**quickXorHash**</span></span> | <span data-ttu-id="ab3cb-126">Строка</span><span class="sxs-lookup"><span data-stu-id="ab3cb-126">String</span></span> | <span data-ttu-id="ab3cb-p105">Особый хэш файла, который можно использовать, чтобы определить, было ли изменено содержимое файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab3cb-p105">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

> <span data-ttu-id="ab3cb-129">**Примечание:** В случаях, когда хэш-значения недоступны, значения хеша для элемента будут обновлены после загрузки элемента.</span><span class="sxs-lookup"><span data-stu-id="ab3cb-129">**Note:** In cases where the hash values are not available, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab3cb-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab3cb-130">JSON representation</span></span>

<span data-ttu-id="ab3cb-131">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab3cb-131">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="ab3cb-132">См. также</span><span class="sxs-lookup"><span data-stu-id="ab3cb-132">See also</span></span>

- <span data-ttu-id="ab3cb-133">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ab3cb-133">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
- <span data-ttu-id="ab3cb-134">Пример вычисления значения **quickXorHash** для файла см. в [фрагменте кода QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).</span><span class="sxs-lookup"><span data-stu-id="ab3cb-134">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>


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
