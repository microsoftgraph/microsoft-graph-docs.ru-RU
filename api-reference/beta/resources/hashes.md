---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Hashes
localization_priority: Normal
ms.openlocfilehash: be7d3b27b1ef22976dc93ea5aecbc2a64031e8b4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506351"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="31511-102">Тип ресурса Hashes</span><span class="sxs-lookup"><span data-stu-id="31511-102">Hashes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31511-103">Ресурс **хэшей** группирует доступных хэши в единую структуру для элемента.</span><span class="sxs-lookup"><span data-stu-id="31511-103">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="31511-104">**Примечание.** Не все службы предоставляют значение для всех свойств хэша в списке.</span><span class="sxs-lookup"><span data-stu-id="31511-104">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="31511-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31511-105">JSON representation</span></span>

<span data-ttu-id="31511-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31511-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="31511-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="31511-107">Properties</span></span>

| <span data-ttu-id="31511-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="31511-108">Property</span></span>         | <span data-ttu-id="31511-109">Тип</span><span class="sxs-lookup"><span data-stu-id="31511-109">Type</span></span>   | <span data-ttu-id="31511-110">Описание</span><span class="sxs-lookup"><span data-stu-id="31511-110">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="31511-111">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="31511-111">**sha1Hash**</span></span>     | <span data-ttu-id="31511-112">String</span><span class="sxs-lookup"><span data-stu-id="31511-112">String</span></span> | <span data-ttu-id="31511-p101">Хэш SHA1 для содержимого файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31511-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="31511-115">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="31511-115">**crc32Hash**</span></span>    | <span data-ttu-id="31511-116">String</span><span class="sxs-lookup"><span data-stu-id="31511-116">String</span></span> | <span data-ttu-id="31511-p102">Значение CRC32 файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31511-p102">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="31511-119">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="31511-119">**quickXorHash**</span></span> | <span data-ttu-id="31511-120">Строка</span><span class="sxs-lookup"><span data-stu-id="31511-120">String</span></span> | <span data-ttu-id="31511-p103">Особый хэш файла, который можно использовать, чтобы определить, было ли изменено содержимое файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31511-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="31511-p104">**Примечание.** В некоторых случаях значения хэша могут быть недоступны. Если это так, значения хэша для определенного элемента будут обновлены после загрузки элемента.</span><span class="sxs-lookup"><span data-stu-id="31511-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="31511-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="31511-125">Remarks</span></span>

<span data-ttu-id="31511-126">В OneDrive для бизнеса и SharePoint Server 2016 значения **sha1Hash** и **crc32Hash** недоступны.</span><span class="sxs-lookup"><span data-stu-id="31511-126">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="31511-127">В OneDrive персональный значение **quickXorHash** недоступно.</span><span class="sxs-lookup"><span data-stu-id="31511-127">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="31511-128">Сведения о том, как вычислить значение **quickXorHash** для файла, см. в [фрагменте кода QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).</span><span class="sxs-lookup"><span data-stu-id="31511-128">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>

<span data-ttu-id="31511-129">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="31511-129">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes",
  "suppressions": [
    "Error: /api-reference/beta/resources/hashes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
