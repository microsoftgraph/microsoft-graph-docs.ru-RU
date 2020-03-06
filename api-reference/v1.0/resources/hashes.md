---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
localization_priority: Normal
title: Тип ресурса Hashes
description: Ресурс хэшей группирует доступных хэши в единую структуру для элемента.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cb852ad01394ac463cb3d23ed404a7956bbf1eea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532912"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="254f5-103">Тип ресурса Hashes</span><span class="sxs-lookup"><span data-stu-id="254f5-103">Hashes resource type</span></span>

<span data-ttu-id="254f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="254f5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="254f5-105">Ресурс **хэшей** группирует доступных хэши в единую структуру для элемента.</span><span class="sxs-lookup"><span data-stu-id="254f5-105">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="254f5-106">**Примечание.** Не все службы предоставляют значение для всех свойств хэша в списке.</span><span class="sxs-lookup"><span data-stu-id="254f5-106">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="254f5-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="254f5-107">JSON representation</span></span>

<span data-ttu-id="254f5-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="254f5-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string (hex)",
  "sha1Hash": "string (hex)",
  "quickXorHash": "string (base64)"
}
```

## <a name="properties"></a><span data-ttu-id="254f5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="254f5-109">Properties</span></span>

| <span data-ttu-id="254f5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="254f5-110">Property</span></span>         | <span data-ttu-id="254f5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="254f5-111">Type</span></span>   | <span data-ttu-id="254f5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="254f5-112">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="254f5-113">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="254f5-113">**sha1Hash**</span></span>     | <span data-ttu-id="254f5-114">String</span><span class="sxs-lookup"><span data-stu-id="254f5-114">String</span></span> | <span data-ttu-id="254f5-p101">Хэш SHA1 для содержимого файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="254f5-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="254f5-117">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="254f5-117">**crc32Hash**</span></span>    | <span data-ttu-id="254f5-118">String</span><span class="sxs-lookup"><span data-stu-id="254f5-118">String</span></span> | <span data-ttu-id="254f5-119">Значение CRC32 файла с прямым порядком байтов (при наличии).</span><span class="sxs-lookup"><span data-stu-id="254f5-119">The CRC32 value of the file in little endian (if available).</span></span> <span data-ttu-id="254f5-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="254f5-120">Read-only.</span></span>            |
| <span data-ttu-id="254f5-121">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="254f5-121">**quickXorHash**</span></span> | <span data-ttu-id="254f5-122">Строка</span><span class="sxs-lookup"><span data-stu-id="254f5-122">String</span></span> | <span data-ttu-id="254f5-p103">Особый хэш файла, который можно использовать, чтобы определить, было ли изменено содержимое файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="254f5-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="254f5-p104">**Примечание.** В некоторых случаях значения хэша могут быть недоступны. Если это так, значения хэша для определенного элемента будут обновлены после загрузки элемента.</span><span class="sxs-lookup"><span data-stu-id="254f5-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="254f5-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="254f5-127">Remarks</span></span>

<span data-ttu-id="254f5-128">В OneDrive для бизнеса и SharePoint Server 2016 значения **sha1Hash** и **crc32Hash** недоступны.</span><span class="sxs-lookup"><span data-stu-id="254f5-128">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="254f5-129">В OneDrive персональный значение **quickXorHash** недоступно.</span><span class="sxs-lookup"><span data-stu-id="254f5-129">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="254f5-130">Сведения о том, как вычислить значение **quickXorHash** для файла, см. в [фрагменте кода QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).</span><span class="sxs-lookup"><span data-stu-id="254f5-130">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>
<span data-ttu-id="254f5-131">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="254f5-131">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
