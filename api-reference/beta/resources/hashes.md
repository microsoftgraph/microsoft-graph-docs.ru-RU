---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Hashes
localization_priority: Normal
ms.openlocfilehash: ff147b45bcdc200e3da5d4a8761d8248fa887271
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853412"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="13023-102">Тип ресурса Hashes</span><span class="sxs-lookup"><span data-stu-id="13023-102">Hashes resource type</span></span>

> <span data-ttu-id="13023-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="13023-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13023-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13023-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13023-105">Ресурс **хэшей** группирует доступных хэши в единую структуру для элемента.</span><span class="sxs-lookup"><span data-stu-id="13023-105">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="13023-106">**Примечание.** Не все службы предоставляют значение для всех свойств хэша в списке.</span><span class="sxs-lookup"><span data-stu-id="13023-106">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="13023-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13023-107">JSON representation</span></span>

<span data-ttu-id="13023-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13023-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="13023-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="13023-109">Properties</span></span>

| <span data-ttu-id="13023-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="13023-110">Property</span></span>         | <span data-ttu-id="13023-111">Тип</span><span class="sxs-lookup"><span data-stu-id="13023-111">Type</span></span>   | <span data-ttu-id="13023-112">Описание</span><span class="sxs-lookup"><span data-stu-id="13023-112">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="13023-113">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="13023-113">**sha1Hash**</span></span>     | <span data-ttu-id="13023-114">String</span><span class="sxs-lookup"><span data-stu-id="13023-114">String</span></span> | <span data-ttu-id="13023-p102">Хэш SHA1 для содержимого файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13023-p102">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="13023-117">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="13023-117">**crc32Hash**</span></span>    | <span data-ttu-id="13023-118">String</span><span class="sxs-lookup"><span data-stu-id="13023-118">String</span></span> | <span data-ttu-id="13023-p103">Значение CRC32 файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13023-p103">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="13023-121">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="13023-121">**quickXorHash**</span></span> | <span data-ttu-id="13023-122">Строка</span><span class="sxs-lookup"><span data-stu-id="13023-122">String</span></span> | <span data-ttu-id="13023-p104">Особый хэш файла, который можно использовать, чтобы определить, было ли изменено содержимое файла (если доступно). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13023-p104">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="13023-p105">**Примечание.** В некоторых случаях значения хэша могут быть недоступны. Если это так, значения хэша для определенного элемента будут обновлены после загрузки элемента.</span><span class="sxs-lookup"><span data-stu-id="13023-p105">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="13023-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="13023-127">Remarks</span></span>

<span data-ttu-id="13023-128">В OneDrive для бизнеса и SharePoint Server 2016 значения **sha1Hash** и **crc32Hash** недоступны.</span><span class="sxs-lookup"><span data-stu-id="13023-128">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="13023-129">В OneDrive персональный значение **quickXorHash** недоступно.</span><span class="sxs-lookup"><span data-stu-id="13023-129">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="13023-130">Сведения о том, как вычислить значение **quickXorHash** для файла, см. в [фрагменте кода QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).</span><span class="sxs-lookup"><span data-stu-id="13023-130">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>

<span data-ttu-id="13023-131">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="13023-131">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
