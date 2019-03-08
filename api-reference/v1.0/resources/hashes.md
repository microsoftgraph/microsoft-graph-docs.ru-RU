---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
localization_priority: Normal
ms.openlocfilehash: abe6fc277f94eb1f66f50f25b894bc41fd038a9b
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480210"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="3fb49-101">Тип ресурса Hashes</span><span class="sxs-lookup"><span data-stu-id="3fb49-101">Hashes resource type</span></span>

<span data-ttu-id="3fb49-102">Ресурс **хэшей** группирует доступных хэши в единую структуру для элемента.</span><span class="sxs-lookup"><span data-stu-id="3fb49-102">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="3fb49-103">**Примечание.** Не все службы предоставляют значение для всех свойств хэша в списке.</span><span class="sxs-lookup"><span data-stu-id="3fb49-103">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3fb49-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3fb49-104">JSON representation</span></span>

<span data-ttu-id="3fb49-105">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3fb49-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3fb49-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3fb49-106">Properties</span></span>

| <span data-ttu-id="3fb49-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fb49-107">Property</span></span>         | <span data-ttu-id="3fb49-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3fb49-108">Type</span></span>   | <span data-ttu-id="3fb49-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3fb49-109">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="3fb49-110">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="3fb49-110">**sha1Hash**</span></span>     | <span data-ttu-id="3fb49-111">String</span><span class="sxs-lookup"><span data-stu-id="3fb49-111">String</span></span> | <span data-ttu-id="3fb49-p101">Хэш SHA1 для содержимого файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3fb49-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="3fb49-114">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="3fb49-114">**crc32Hash**</span></span>    | <span data-ttu-id="3fb49-115">String</span><span class="sxs-lookup"><span data-stu-id="3fb49-115">String</span></span> | <span data-ttu-id="3fb49-116">Значение CRC32 файла с прямым порядком байтов (при наличии).</span><span class="sxs-lookup"><span data-stu-id="3fb49-116">The CRC32 value of the file in little endian (if available).</span></span> <span data-ttu-id="3fb49-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3fb49-117">Read-only.</span></span>            |
| <span data-ttu-id="3fb49-118">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="3fb49-118">**quickXorHash**</span></span> | <span data-ttu-id="3fb49-119">Строка</span><span class="sxs-lookup"><span data-stu-id="3fb49-119">String</span></span> | <span data-ttu-id="3fb49-p103">Особый хэш файла, который можно использовать, чтобы определить, было ли изменено содержимое файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3fb49-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="3fb49-p104">**Примечание.** В некоторых случаях значения хэша могут быть недоступны. Если это так, значения хэша для определенного элемента будут обновлены после загрузки элемента.</span><span class="sxs-lookup"><span data-stu-id="3fb49-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="3fb49-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="3fb49-124">Remarks</span></span>

<span data-ttu-id="3fb49-125">В OneDrive для бизнеса и SharePoint Server 2016 значения **sha1Hash** и **crc32Hash** недоступны.</span><span class="sxs-lookup"><span data-stu-id="3fb49-125">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="3fb49-126">В OneDrive персональный значение **quickXorHash** недоступно.</span><span class="sxs-lookup"><span data-stu-id="3fb49-126">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="3fb49-127">Сведения о том, как вычислить значение **quickXorHash** для файла, см. в [фрагменте кода QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).</span><span class="sxs-lookup"><span data-stu-id="3fb49-127">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>
<span data-ttu-id="3fb49-128">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="3fb49-128">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
