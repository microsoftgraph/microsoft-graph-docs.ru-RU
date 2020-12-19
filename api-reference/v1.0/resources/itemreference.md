---
author: JeremyKelley
ms.date: 09/10/2017
title: ItemReference
localization_priority: Normal
description: Ресурс ItemReference предоставляет сведения, необходимые для обращения к ресурсу DriveItem через API.
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: dd24f0d1fc0a5f5db576f5eea89b8205ff55b2b7
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714258"
---
# <a name="itemreference-resource-type"></a><span data-ttu-id="ea8b6-103">Тип ресурса ItemReference</span><span class="sxs-lookup"><span data-stu-id="ea8b6-103">ItemReference resource type</span></span>

<span data-ttu-id="ea8b6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea8b6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea8b6-105">Ресурс **ItemReference** предоставляет сведения, необходимые для обращения к ресурсу [DriveItem](driveitem.md) через API.</span><span class="sxs-lookup"><span data-stu-id="ea8b6-105">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea8b6-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea8b6-106">JSON representation</span></span>

<span data-ttu-id="ea8b6-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="ea8b6-107">Here is a JSON representation of the resource</span></span>

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
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="ea8b6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea8b6-108">Properties</span></span>

| <span data-ttu-id="ea8b6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea8b6-109">Property</span></span>      | <span data-ttu-id="ea8b6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ea8b6-110">Type</span></span>              | <span data-ttu-id="ea8b6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ea8b6-111">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="ea8b6-112">driveId</span><span class="sxs-lookup"><span data-stu-id="ea8b6-112">driveId</span></span>       | <span data-ttu-id="ea8b6-113">String</span><span class="sxs-lookup"><span data-stu-id="ea8b6-113">String</span></span>            | <span data-ttu-id="ea8b6-p101">Уникальный идентификатор экземпляра диска, содержащего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ea8b6-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>
| <span data-ttu-id="ea8b6-116">driveType</span><span class="sxs-lookup"><span data-stu-id="ea8b6-116">driveType</span></span>     | <span data-ttu-id="ea8b6-117">Строка</span><span class="sxs-lookup"><span data-stu-id="ea8b6-117">String</span></span>            | <span data-ttu-id="ea8b6-118">Служит для идентификации типа для объекта drive.</span><span class="sxs-lookup"><span data-stu-id="ea8b6-118">Identifies the type of drive.</span></span> <span data-ttu-id="ea8b6-119">Сведения о возможных значениях см. в статье, посвященной ресурсу [drive][].</span><span class="sxs-lookup"><span data-stu-id="ea8b6-119">See [drive][] resource for values.</span></span>
| <span data-ttu-id="ea8b6-120">id</span><span class="sxs-lookup"><span data-stu-id="ea8b6-120">id</span></span>            | <span data-ttu-id="ea8b6-121">String</span><span class="sxs-lookup"><span data-stu-id="ea8b6-121">String</span></span>            | <span data-ttu-id="ea8b6-p103">Уникальный идентификатор элемента на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ea8b6-p103">Unique identifier of the item in the drive. Read-only.</span></span>
| <span data-ttu-id="ea8b6-124">name</span><span class="sxs-lookup"><span data-stu-id="ea8b6-124">name</span></span>          | <span data-ttu-id="ea8b6-125">String</span><span class="sxs-lookup"><span data-stu-id="ea8b6-125">String</span></span>            | <span data-ttu-id="ea8b6-p104">Имя элемента, на который направлена ссылка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ea8b6-p104">The name of the item being referenced. Read-only.</span></span>
| <span data-ttu-id="ea8b6-128">path</span><span class="sxs-lookup"><span data-stu-id="ea8b6-128">path</span></span>          | <span data-ttu-id="ea8b6-129">String</span><span class="sxs-lookup"><span data-stu-id="ea8b6-129">String</span></span>            | <span data-ttu-id="ea8b6-p105">Путь, по которому можно перейти к элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ea8b6-p105">Path that can be used to navigate to the item. Read-only.</span></span>
| <span data-ttu-id="ea8b6-132">shareId</span><span class="sxs-lookup"><span data-stu-id="ea8b6-132">shareId</span></span>       | <span data-ttu-id="ea8b6-133">String</span><span class="sxs-lookup"><span data-stu-id="ea8b6-133">String</span></span>            | <span data-ttu-id="ea8b6-134">Уникальный идентификатор общего ресурса, доступ к которому можно получить с помощью API [Shares][].</span><span class="sxs-lookup"><span data-stu-id="ea8b6-134">A unique identifier for a shared resource that can be accessed via the [Shares][] API.</span></span>
| <span data-ttu-id="ea8b6-135">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ea8b6-135">sharepointIds</span></span> | <span data-ttu-id="ea8b6-136">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="ea8b6-136">[sharepointIds][]</span></span> | <span data-ttu-id="ea8b6-p106">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ea8b6-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="ea8b6-139">siteId</span><span class="sxs-lookup"><span data-stu-id="ea8b6-139">siteId</span></span>        | <span data-ttu-id="ea8b6-140">String</span><span class="sxs-lookup"><span data-stu-id="ea8b6-140">String</span></span>            | <span data-ttu-id="ea8b6-141">Для OneDrive для бизнеса и SharePoint это свойство представляет собой ИД сайта, который содержит родительную библиотеку документов ресурса driveItem.</span><span class="sxs-lookup"><span data-stu-id="ea8b6-141">For OneDrive for Business and SharePoint, this property represents the ID of the site that contains the parent document library of the driveItem resource.</span></span> <span data-ttu-id="ea8b6-142">Это значение такое же, как свойство id этого [ресурса][] сайта.</span><span class="sxs-lookup"><span data-stu-id="ea8b6-142">The value is the same as the id property of that [site][] resource.</span></span> <span data-ttu-id="ea8b6-143">Это [непрозрачной строки, которая состоит из трех идентификаторов](/graph/api/resources/site#id-property) сайта.</span><span class="sxs-lookup"><span data-stu-id="ea8b6-143">It is an [opaque string that consists of three identifiers](/graph/api/resources/site#id-property) of the site.</span></span> <br><span data-ttu-id="ea8b6-144">В OneDrive это свойство не заполняется.</span><span class="sxs-lookup"><span data-stu-id="ea8b6-144">For OneDrive, this property is not populated.</span></span>

[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares-get.md
[site]: ../resources/site.md

## <a name="remarks"></a><span data-ttu-id="ea8b6-149">Замечания</span><span class="sxs-lookup"><span data-stu-id="ea8b6-149">Remarks</span></span>

<span data-ttu-id="ea8b6-150">Чтобы обратиться к элементу **driveItem** из ресурса **itemReference**, составьте URL-адрес в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="ea8b6-150">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="ea8b6-151">Значение **path** — это путь к API относительно целевого диска, например: `/drive/root:/Documents/myfile.docx`.</span><span class="sxs-lookup"><span data-stu-id="ea8b6-151">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="ea8b6-152">Чтобы получить удобочитаемый путь для навигации, вы можете пропустить все до первого символа `:` в строке пути.</span><span class="sxs-lookup"><span data-stu-id="ea8b6-152">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

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

