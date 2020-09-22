---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ItemReference
localization_priority: Normal
description: Ресурс ItemReference предоставляет сведения, необходимые для обращения к ресурсу DriveItem через API.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a13fb5a3606b72c96a15317a9a7b1d5844184f4c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009228"
---
# <a name="itemreference-resource-type"></a><span data-ttu-id="cfb7c-103">Тип ресурса ItemReference</span><span class="sxs-lookup"><span data-stu-id="cfb7c-103">ItemReference resource type</span></span>

<span data-ttu-id="cfb7c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfb7c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cfb7c-105">Ресурс **ItemReference** предоставляет сведения, необходимые для обращения к ресурсу [DriveItem](driveitem.md) через API.</span><span class="sxs-lookup"><span data-stu-id="cfb7c-105">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfb7c-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cfb7c-106">JSON representation</span></span>

<span data-ttu-id="cfb7c-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="cfb7c-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path", "shareId", "sharepointIds" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "driveType": "personal | business | documentLibrary",
  "id": "string",
  "name": "string",
  "path": "string",
  "shareId": "string",
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" }
}
```

## <a name="properties"></a><span data-ttu-id="cfb7c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cfb7c-108">Properties</span></span>

| <span data-ttu-id="cfb7c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cfb7c-109">Property</span></span>      | <span data-ttu-id="cfb7c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cfb7c-110">Type</span></span>              | <span data-ttu-id="cfb7c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cfb7c-111">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="cfb7c-112">driveId</span><span class="sxs-lookup"><span data-stu-id="cfb7c-112">driveId</span></span>       | <span data-ttu-id="cfb7c-113">String</span><span class="sxs-lookup"><span data-stu-id="cfb7c-113">String</span></span>            | <span data-ttu-id="cfb7c-p101">Уникальный идентификатор экземпляра диска, содержащего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cfb7c-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>
| <span data-ttu-id="cfb7c-116">driveType</span><span class="sxs-lookup"><span data-stu-id="cfb7c-116">driveType</span></span>     | <span data-ttu-id="cfb7c-117">Строка</span><span class="sxs-lookup"><span data-stu-id="cfb7c-117">String</span></span>            | <span data-ttu-id="cfb7c-118">Служит для идентификации типа для объекта drive.</span><span class="sxs-lookup"><span data-stu-id="cfb7c-118">Identifies the type of drive.</span></span> <span data-ttu-id="cfb7c-119">Сведения о возможных значениях см. в статье, посвященной ресурсу [drive][].</span><span class="sxs-lookup"><span data-stu-id="cfb7c-119">See [drive][] resource for values.</span></span>
| <span data-ttu-id="cfb7c-120">id</span><span class="sxs-lookup"><span data-stu-id="cfb7c-120">id</span></span>            | <span data-ttu-id="cfb7c-121">String</span><span class="sxs-lookup"><span data-stu-id="cfb7c-121">String</span></span>            | <span data-ttu-id="cfb7c-p103">Уникальный идентификатор элемента на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cfb7c-p103">Unique identifier of the item in the drive. Read-only.</span></span>
| <span data-ttu-id="cfb7c-124">name</span><span class="sxs-lookup"><span data-stu-id="cfb7c-124">name</span></span>          | <span data-ttu-id="cfb7c-125">String</span><span class="sxs-lookup"><span data-stu-id="cfb7c-125">String</span></span>            | <span data-ttu-id="cfb7c-p104">Имя элемента, на который направлена ссылка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cfb7c-p104">The name of the item being referenced. Read-only.</span></span>
| <span data-ttu-id="cfb7c-128">path</span><span class="sxs-lookup"><span data-stu-id="cfb7c-128">path</span></span>          | <span data-ttu-id="cfb7c-129">String</span><span class="sxs-lookup"><span data-stu-id="cfb7c-129">String</span></span>            | <span data-ttu-id="cfb7c-p105">Путь, по которому можно перейти к элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cfb7c-p105">Path that can be used to navigate to the item. Read-only.</span></span>
| <span data-ttu-id="cfb7c-132">shareId</span><span class="sxs-lookup"><span data-stu-id="cfb7c-132">shareId</span></span>       | <span data-ttu-id="cfb7c-133">String</span><span class="sxs-lookup"><span data-stu-id="cfb7c-133">String</span></span>            | <span data-ttu-id="cfb7c-134">Уникальный идентификатор общего ресурса, доступ к которому можно получить с помощью API [Shares][].</span><span class="sxs-lookup"><span data-stu-id="cfb7c-134">A unique identifier for a shared resource that can be accessed via the [Shares][] API.</span></span>
| <span data-ttu-id="cfb7c-135">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="cfb7c-135">sharepointIds</span></span> | <span data-ttu-id="cfb7c-136">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="cfb7c-136">[sharepointIds][]</span></span> | <span data-ttu-id="cfb7c-p106">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cfb7c-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>

[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares-get.md

## <a name="remarks"></a><span data-ttu-id="cfb7c-142">Замечания</span><span class="sxs-lookup"><span data-stu-id="cfb7c-142">Remarks</span></span>

<span data-ttu-id="cfb7c-143">Чтобы обратиться к элементу **driveItem** из ресурса **itemReference**, составьте URL-адрес в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="cfb7c-143">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="cfb7c-144">Значение **path** — это путь к API относительно целевого диска, например: `/drive/root:/Documents/myfile.docx`.</span><span class="sxs-lookup"><span data-stu-id="cfb7c-144">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="cfb7c-145">Чтобы получить удобочитаемый путь для навигации, вы можете пропустить все до первого символа `:` в строке пути.</span><span class="sxs-lookup"><span data-stu-id="cfb7c-145">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ItemReference returns a pointer to another item.",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/itemreference.md:
      Found potential enums in resource example that weren't defined in a table:(personal,business,documentLibrary) are in resource, but () are in table"
  ],
  "tocPath": "Resources/ItemReference"
} -->

