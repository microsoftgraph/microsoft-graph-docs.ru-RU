---
author: JeremyKelley
description: Ресурс ItemReference предоставляет сведения, необходимые для обращения к ресурсу DriveItem через API.
ms.date: 09/10/2017
title: ItemReference
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 434e3ed1da1f7536224e27b619cedf3bbef5f20e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967065"
---
# <a name="itemreference-resource-type"></a><span data-ttu-id="e121b-103">Тип ресурса ItemReference</span><span class="sxs-lookup"><span data-stu-id="e121b-103">ItemReference resource type</span></span>

<span data-ttu-id="e121b-104">Ресурс **ItemReference** предоставляет сведения, необходимые для обращения к ресурсу [DriveItem](driveitem.md) через API.</span><span class="sxs-lookup"><span data-stu-id="e121b-104">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e121b-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e121b-105">JSON representation</span></span>

<span data-ttu-id="e121b-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="e121b-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="e121b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e121b-107">Properties</span></span>

| <span data-ttu-id="e121b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e121b-108">Property</span></span>      | <span data-ttu-id="e121b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e121b-109">Type</span></span>              | <span data-ttu-id="e121b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e121b-110">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="e121b-111">driveId</span><span class="sxs-lookup"><span data-stu-id="e121b-111">driveId</span></span>       | <span data-ttu-id="e121b-112">Строка</span><span class="sxs-lookup"><span data-stu-id="e121b-112">String</span></span>            | <span data-ttu-id="e121b-p101">Уникальный идентификатор экземпляра диска, содержащего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e121b-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>
| <span data-ttu-id="e121b-115">driveType</span><span class="sxs-lookup"><span data-stu-id="e121b-115">driveType</span></span>     | <span data-ttu-id="e121b-116">String</span><span class="sxs-lookup"><span data-stu-id="e121b-116">String</span></span>            | <span data-ttu-id="e121b-117">Служит для идентификации типа для объекта drive.</span><span class="sxs-lookup"><span data-stu-id="e121b-117">Identifies the type of drive.</span></span> <span data-ttu-id="e121b-118">Сведения о возможных значениях см. в статье, посвященной ресурсу [drive][].</span><span class="sxs-lookup"><span data-stu-id="e121b-118">See [drive][] resource for values.</span></span>
| <span data-ttu-id="e121b-119">id</span><span class="sxs-lookup"><span data-stu-id="e121b-119">id</span></span>            | <span data-ttu-id="e121b-120">String</span><span class="sxs-lookup"><span data-stu-id="e121b-120">String</span></span>            | <span data-ttu-id="e121b-p103">Уникальный идентификатор элемента на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e121b-p103">Unique identifier of the item in the drive. Read-only.</span></span>
| <span data-ttu-id="e121b-123">name</span><span class="sxs-lookup"><span data-stu-id="e121b-123">name</span></span>          | <span data-ttu-id="e121b-124">String</span><span class="sxs-lookup"><span data-stu-id="e121b-124">String</span></span>            | <span data-ttu-id="e121b-p104">Имя элемента, на который направлена ссылка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e121b-p104">The name of the item being referenced. Read-only.</span></span>
| <span data-ttu-id="e121b-127">path</span><span class="sxs-lookup"><span data-stu-id="e121b-127">path</span></span>          | <span data-ttu-id="e121b-128">String</span><span class="sxs-lookup"><span data-stu-id="e121b-128">String</span></span>            | <span data-ttu-id="e121b-p105">Путь, по которому можно перейти к элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e121b-p105">Path that can be used to navigate to the item. Read-only.</span></span>
| <span data-ttu-id="e121b-131">shareId</span><span class="sxs-lookup"><span data-stu-id="e121b-131">shareId</span></span>       | <span data-ttu-id="e121b-132">Строка</span><span class="sxs-lookup"><span data-stu-id="e121b-132">String</span></span>            | <span data-ttu-id="e121b-133">Уникальный идентификатор общего ресурса, доступ к которому можно получить с помощью API [Shares][].</span><span class="sxs-lookup"><span data-stu-id="e121b-133">A unique identifier for a shared resource that can be accessed via the [Shares][] API.</span></span>
| <span data-ttu-id="e121b-134">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="e121b-134">sharepointIds</span></span> | <span data-ttu-id="e121b-135">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="e121b-135">[sharepointIds][]</span></span> | <span data-ttu-id="e121b-p106">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e121b-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>

[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares-get.md

## <a name="remarks"></a><span data-ttu-id="e121b-141">Замечания</span><span class="sxs-lookup"><span data-stu-id="e121b-141">Remarks</span></span>

<span data-ttu-id="e121b-142">Чтобы обратиться к элементу **driveItem** из ресурса **itemReference**, составьте URL-адрес в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="e121b-142">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="e121b-143">Значение **path** — это путь к API относительно целевого диска, например: `/drive/root:/Documents/myfile.docx`.</span><span class="sxs-lookup"><span data-stu-id="e121b-143">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="e121b-144">Чтобы получить удобочитаемый путь для навигации, вы можете пропустить все до первого символа `:` в строке пути.</span><span class="sxs-lookup"><span data-stu-id="e121b-144">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ItemReference returns a pointer to another item.",
  "section": "documentation",
  "tocPath": "Resources/ItemReference"
} -->
