---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
localization_priority: Normal
ms.openlocfilehash: 3ed0023e80457598bd80b068156b60a5ace4984b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830487"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="ae8ff-101">Тип ресурса хэшей</span><span class="sxs-lookup"><span data-stu-id="ae8ff-101">Hashes resource type</span></span>

<span data-ttu-id="ae8ff-102">Ресурс **хэшей** группирует доступных хэши в единую структуру для элемента.</span><span class="sxs-lookup"><span data-stu-id="ae8ff-102">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="ae8ff-103">**Примечание.** Не все службы предоставляют значение для всех свойств хэша в списке.</span><span class="sxs-lookup"><span data-stu-id="ae8ff-103">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae8ff-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae8ff-104">JSON representation</span></span>

<span data-ttu-id="ae8ff-105">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae8ff-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ae8ff-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae8ff-106">Properties</span></span>

| <span data-ttu-id="ae8ff-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae8ff-107">Property</span></span>         | <span data-ttu-id="ae8ff-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ae8ff-108">Type</span></span>   | <span data-ttu-id="ae8ff-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ae8ff-109">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="ae8ff-110">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="ae8ff-110">**sha1Hash**</span></span>     | <span data-ttu-id="ae8ff-111">String</span><span class="sxs-lookup"><span data-stu-id="ae8ff-111">String</span></span> | <span data-ttu-id="ae8ff-p101">Хэш SHA1 для содержимого файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ae8ff-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="ae8ff-114">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="ae8ff-114">**crc32Hash**</span></span>    | <span data-ttu-id="ae8ff-115">String</span><span class="sxs-lookup"><span data-stu-id="ae8ff-115">String</span></span> | <span data-ttu-id="ae8ff-116">Значение CRC32 файла в прямой порядок (при наличии).</span><span class="sxs-lookup"><span data-stu-id="ae8ff-116">The CRC32 value of the file in little endian (if available).</span></span> <span data-ttu-id="ae8ff-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ae8ff-117">Read-only.</span></span>            |
| <span data-ttu-id="ae8ff-118">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="ae8ff-118">**quickXorHash**</span></span> | <span data-ttu-id="ae8ff-119">Строка</span><span class="sxs-lookup"><span data-stu-id="ae8ff-119">String</span></span> | <span data-ttu-id="ae8ff-p103">Особый хэш файла, который можно использовать, чтобы определить, было ли изменено содержимое файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ae8ff-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="ae8ff-p104">**Примечание.** В некоторых случаях значения хэша могут быть недоступны. Если это так, значения хэша для определенного элемента будут обновлены после загрузки элемента.</span><span class="sxs-lookup"><span data-stu-id="ae8ff-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="ae8ff-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="ae8ff-124">Remarks</span></span>

<span data-ttu-id="ae8ff-125">В OneDrive для бизнеса и SharePoint Server 2016 значения **sha1Hash** и **crc32Hash** недоступны.</span><span class="sxs-lookup"><span data-stu-id="ae8ff-125">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="ae8ff-126">В OneDrive персональный значение **quickXorHash** недоступно.</span><span class="sxs-lookup"><span data-stu-id="ae8ff-126">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="ae8ff-127">Сведения о том, как вычислить значение **quickXorHash** для файла, см. в [фрагменте кода QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).</span><span class="sxs-lookup"><span data-stu-id="ae8ff-127">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>
<span data-ttu-id="ae8ff-128">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ae8ff-128">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
