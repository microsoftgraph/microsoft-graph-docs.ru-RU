---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
ms.openlocfilehash: 9de6923146b915207fc771721d7aeb6767e9f99e
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="hashes-resource-type"></a><span data-ttu-id="fdc7d-101">Тип ресурса хэшей</span><span class="sxs-lookup"><span data-stu-id="fdc7d-101">Hashes resource type</span></span>

<span data-ttu-id="fdc7d-102">Ресурс **хэшей** группирует доступных хэши в единую структуру для элемента.</span><span class="sxs-lookup"><span data-stu-id="fdc7d-102">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="fdc7d-103">**Примечание.** Не все службы предоставляют значение для всех свойств хэша в списке.</span><span class="sxs-lookup"><span data-stu-id="fdc7d-103">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fdc7d-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fdc7d-104">JSON representation</span></span>

<span data-ttu-id="fdc7d-105">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdc7d-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="fdc7d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fdc7d-106">Properties</span></span>

| <span data-ttu-id="fdc7d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdc7d-107">Property</span></span>         | <span data-ttu-id="fdc7d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fdc7d-108">Type</span></span>   | <span data-ttu-id="fdc7d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fdc7d-109">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="fdc7d-110">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="fdc7d-110">**sha1Hash**</span></span>     | <span data-ttu-id="fdc7d-111">String</span><span class="sxs-lookup"><span data-stu-id="fdc7d-111">String</span></span> | <span data-ttu-id="fdc7d-p101">Хэш SHA1 для содержимого файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fdc7d-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="fdc7d-114">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="fdc7d-114">**crc32Hash**</span></span>    | <span data-ttu-id="fdc7d-115">String</span><span class="sxs-lookup"><span data-stu-id="fdc7d-115">String</span></span> | <span data-ttu-id="fdc7d-p102">Значение CRC32 файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fdc7d-p102">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="fdc7d-118">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="fdc7d-118">**quickXorHash**</span></span> | <span data-ttu-id="fdc7d-119">Строка</span><span class="sxs-lookup"><span data-stu-id="fdc7d-119">String</span></span> | <span data-ttu-id="fdc7d-p103">Особый хэш файла, который можно использовать, чтобы определить, было ли изменено содержимое файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fdc7d-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="fdc7d-p104">**Примечание.** В некоторых случаях значения хэша могут быть недоступны. Если это так, значения хэша для определенного элемента будут обновлены после загрузки элемента.</span><span class="sxs-lookup"><span data-stu-id="fdc7d-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="fdc7d-124">Заметки</span><span class="sxs-lookup"><span data-stu-id="fdc7d-124">Remarks</span></span>

<span data-ttu-id="fdc7d-125">В OneDrive для бизнеса и SharePoint Server 2016 значения **sha1Hash** и **crc32Hash** недоступны.</span><span class="sxs-lookup"><span data-stu-id="fdc7d-125">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="fdc7d-126">В OneDrive персональный значение **quickXorHash** недоступно.</span><span class="sxs-lookup"><span data-stu-id="fdc7d-126">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="fdc7d-127">Пример вычисления значения **quickXorHash** для файла см. в [фрагменте кода QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).</span><span class="sxs-lookup"><span data-stu-id="fdc7d-127">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>
<span data-ttu-id="fdc7d-128">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="fdc7d-128">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
