---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Файл
localization_priority: Normal
description: Ресурс File — это единая структура, объединяющая элементы данных, связанные с файлами.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 51ec91a635db2ca259ba84cea29304e4e6ac7cbb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030375"
---
# <a name="file-resource-type"></a><span data-ttu-id="41cb4-103">Тип ресурса file</span><span class="sxs-lookup"><span data-stu-id="41cb4-103">File resource type</span></span>

<span data-ttu-id="41cb4-104">Ресурс **File** — это единая структура, объединяющая элементы данных, связанные с файлами.</span><span class="sxs-lookup"><span data-stu-id="41cb4-104">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="41cb4-p101">Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **file**, то этот ресурс представляет файл. Помимо других свойств, у файлов есть связь **content**, которая содержит байтовый поток файла.</span><span class="sxs-lookup"><span data-stu-id="41cb4-p101">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="41cb4-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="41cb4-107">JSON representation</span></span>

<span data-ttu-id="41cb4-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41cb4-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.file"
}-->

```json
{
  "hashes": {"@odata.type": "microsoft.graph.hashes"},
  "mimeType": "string"
}
```

## <a name="properties"></a><span data-ttu-id="41cb4-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="41cb4-109">Properties</span></span>

| <span data-ttu-id="41cb4-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="41cb4-110">Property</span></span> | <span data-ttu-id="41cb4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="41cb4-111">Type</span></span>                    | <span data-ttu-id="41cb4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="41cb4-112">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="41cb4-113">hashes</span><span class="sxs-lookup"><span data-stu-id="41cb4-113">hashes</span></span>   | [<span data-ttu-id="41cb4-114">Hashes</span><span class="sxs-lookup"><span data-stu-id="41cb4-114">Hashes</span></span>](hashes.md) | <span data-ttu-id="41cb4-p102">Хэши двоичного содержимого файла (если они доступны). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41cb4-p102">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="41cb4-117">mimeType</span><span class="sxs-lookup"><span data-stu-id="41cb4-117">mimeType</span></span> | <span data-ttu-id="41cb4-118">string</span><span class="sxs-lookup"><span data-stu-id="41cb4-118">string</span></span>                  | <span data-ttu-id="41cb4-p103">Тип MIME файла. Он определяется логикой на сервере и может не совпадать со значением, предоставленным при отправке файла. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41cb4-p103">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="41cb4-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="41cb4-122">Remarks</span></span> 

<span data-ttu-id="41cb4-123">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="41cb4-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
