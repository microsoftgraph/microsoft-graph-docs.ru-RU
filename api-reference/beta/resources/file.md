---
author: JeremyKelley
description: Ресурс File — это единая структура, объединяющая элементы данных, связанные с файлами.
ms.date: 09/10/2017
title: File
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: aaf662575552a37d28e9a429297f8f58f825b6e6
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291162"
---
# <a name="file-resource-type"></a><span data-ttu-id="55533-103">Тип ресурса file</span><span class="sxs-lookup"><span data-stu-id="55533-103">File resource type</span></span>

<span data-ttu-id="55533-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55533-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55533-105">Ресурс **File** — это единая структура, объединяющая элементы данных, связанные с файлами.</span><span class="sxs-lookup"><span data-stu-id="55533-105">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="55533-p101">Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **file**, то этот ресурс представляет файл. Помимо других свойств, у файлов есть связь **content**, которая содержит байтовый поток файла.</span><span class="sxs-lookup"><span data-stu-id="55533-p101">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="55533-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55533-108">JSON representation</span></span>

<span data-ttu-id="55533-109">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55533-109">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="55533-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="55533-110">Properties</span></span>

| <span data-ttu-id="55533-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="55533-111">Property</span></span> | <span data-ttu-id="55533-112">Тип</span><span class="sxs-lookup"><span data-stu-id="55533-112">Type</span></span>                    | <span data-ttu-id="55533-113">Описание</span><span class="sxs-lookup"><span data-stu-id="55533-113">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="55533-114">hashes</span><span class="sxs-lookup"><span data-stu-id="55533-114">hashes</span></span>   | [<span data-ttu-id="55533-115">hashes</span><span class="sxs-lookup"><span data-stu-id="55533-115">hashes</span></span>](hashes.md) | <span data-ttu-id="55533-p102">Хэши двоичного содержимого файла (если они доступны). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55533-p102">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="55533-118">mimeType</span><span class="sxs-lookup"><span data-stu-id="55533-118">mimeType</span></span> | <span data-ttu-id="55533-119">string</span><span class="sxs-lookup"><span data-stu-id="55533-119">string</span></span>                  | <span data-ttu-id="55533-p103">Тип MIME файла. Он определяется логикой на сервере и может не совпадать со значением, предоставленным при отправке файла. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55533-p103">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="55533-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="55533-123">Remarks</span></span> 

<span data-ttu-id="55533-124">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="55533-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File",
  "suppressions": []
}
-->
