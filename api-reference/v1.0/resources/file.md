---
author: JeremyKelley
ms.date: 09/10/2017
title: Файл ресурса СИПЕ
localization_priority: Normal
description: Ресурс File — это единая структура, объединяющая элементы данных, связанные с файлами.
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 2d44d912116f517a67cce36811a1cacf59c32270
ms.sourcegitcommit: f26428bce3034e206b901e9c747cffcf64b55882
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47651318"
---
# <a name="file-resource-type"></a><span data-ttu-id="53600-103">Тип ресурса file</span><span class="sxs-lookup"><span data-stu-id="53600-103">File resource type</span></span>

<span data-ttu-id="53600-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53600-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="53600-105">Ресурс **File** — это единая структура, объединяющая элементы данных, связанные с файлами.</span><span class="sxs-lookup"><span data-stu-id="53600-105">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="53600-106">Если [**DriveItem**](driveitem.md) имеет аспект **File** , отличный от NULL, элемент представляет файл.</span><span class="sxs-lookup"><span data-stu-id="53600-106">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents a file.</span></span>
<span data-ttu-id="53600-107">Помимо других свойств, у файлов есть связь **content**, которая содержит байтовый поток файла.</span><span class="sxs-lookup"><span data-stu-id="53600-107">In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="53600-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53600-108">JSON representation</span></span>

<span data-ttu-id="53600-109">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53600-109">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="53600-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="53600-110">Properties</span></span>

| <span data-ttu-id="53600-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="53600-111">Property</span></span> | <span data-ttu-id="53600-112">Тип</span><span class="sxs-lookup"><span data-stu-id="53600-112">Type</span></span>                    | <span data-ttu-id="53600-113">Описание</span><span class="sxs-lookup"><span data-stu-id="53600-113">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="53600-114">hashes</span><span class="sxs-lookup"><span data-stu-id="53600-114">hashes</span></span>   | [<span data-ttu-id="53600-115">Hashes</span><span class="sxs-lookup"><span data-stu-id="53600-115">Hashes</span></span>](hashes.md) | <span data-ttu-id="53600-p102">Хэши двоичного содержимого файла (если они доступны). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53600-p102">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="53600-118">mimeType</span><span class="sxs-lookup"><span data-stu-id="53600-118">mimeType</span></span> | <span data-ttu-id="53600-119">string</span><span class="sxs-lookup"><span data-stu-id="53600-119">string</span></span>                  | <span data-ttu-id="53600-p103">Тип MIME файла. Он определяется логикой на сервере и может не совпадать со значением, предоставленным при отправке файла. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53600-p103">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="53600-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="53600-123">Remarks</span></span> 

<span data-ttu-id="53600-124">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="53600-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
