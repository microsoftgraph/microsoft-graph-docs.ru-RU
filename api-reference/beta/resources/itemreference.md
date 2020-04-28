---
author: JeremyKelley
description: Ресурс ItemReference предоставляет сведения, необходимые для обращения к ресурсу DriveItem через API.
ms.date: 09/10/2017
title: ItemReference
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 4f9b061757405f284e367cc4311230c76515a086
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523053"
---
# <a name="itemreference-resource-type"></a><span data-ttu-id="b6df2-103">Тип ресурса ItemReference</span><span class="sxs-lookup"><span data-stu-id="b6df2-103">ItemReference resource type</span></span>

<span data-ttu-id="b6df2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6df2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b6df2-105">Ресурс **ItemReference** предоставляет сведения, необходимые для обращения к ресурсу [DriveItem](driveitem.md) через API.</span><span class="sxs-lookup"><span data-stu-id="b6df2-105">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6df2-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6df2-106">JSON representation</span></span>

<span data-ttu-id="b6df2-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="b6df2-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="b6df2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6df2-108">Properties</span></span>

| <span data-ttu-id="b6df2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6df2-109">Property</span></span>      | <span data-ttu-id="b6df2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b6df2-110">Type</span></span>              | <span data-ttu-id="b6df2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b6df2-111">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="b6df2-112">driveId</span><span class="sxs-lookup"><span data-stu-id="b6df2-112">driveId</span></span>       | <span data-ttu-id="b6df2-113">Строка</span><span class="sxs-lookup"><span data-stu-id="b6df2-113">String</span></span>            | <span data-ttu-id="b6df2-p101">Уникальный идентификатор экземпляра диска, содержащего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6df2-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>
| <span data-ttu-id="b6df2-116">driveType</span><span class="sxs-lookup"><span data-stu-id="b6df2-116">driveType</span></span>     | <span data-ttu-id="b6df2-117">String</span><span class="sxs-lookup"><span data-stu-id="b6df2-117">String</span></span>            | <span data-ttu-id="b6df2-118">Служит для идентификации типа для объекта drive.</span><span class="sxs-lookup"><span data-stu-id="b6df2-118">Identifies the type of drive.</span></span> <span data-ttu-id="b6df2-119">Сведения о возможных значениях см. в статье, посвященной ресурсу [drive][].</span><span class="sxs-lookup"><span data-stu-id="b6df2-119">See [drive][] resource for values.</span></span>
| <span data-ttu-id="b6df2-120">id</span><span class="sxs-lookup"><span data-stu-id="b6df2-120">id</span></span>            | <span data-ttu-id="b6df2-121">String</span><span class="sxs-lookup"><span data-stu-id="b6df2-121">String</span></span>            | <span data-ttu-id="b6df2-p103">Уникальный идентификатор элемента на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6df2-p103">Unique identifier of the item in the drive. Read-only.</span></span>
| <span data-ttu-id="b6df2-124">name</span><span class="sxs-lookup"><span data-stu-id="b6df2-124">name</span></span>          | <span data-ttu-id="b6df2-125">Строка</span><span class="sxs-lookup"><span data-stu-id="b6df2-125">String</span></span>            | <span data-ttu-id="b6df2-p104">Имя элемента, на который направлена ссылка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6df2-p104">The name of the item being referenced. Read-only.</span></span>
| <span data-ttu-id="b6df2-128">path</span><span class="sxs-lookup"><span data-stu-id="b6df2-128">path</span></span>          | <span data-ttu-id="b6df2-129">String</span><span class="sxs-lookup"><span data-stu-id="b6df2-129">String</span></span>            | <span data-ttu-id="b6df2-p105">Путь, по которому можно перейти к элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6df2-p105">Path that can be used to navigate to the item. Read-only.</span></span>
| <span data-ttu-id="b6df2-132">shareId</span><span class="sxs-lookup"><span data-stu-id="b6df2-132">shareId</span></span>       | <span data-ttu-id="b6df2-133">String</span><span class="sxs-lookup"><span data-stu-id="b6df2-133">String</span></span>            | <span data-ttu-id="b6df2-134">Уникальный идентификатор общего ресурса, доступ к которому можно получить с помощью API [Shares][].</span><span class="sxs-lookup"><span data-stu-id="b6df2-134">A unique identifier for a shared resource that can be accessed via the [Shares][] API.</span></span>
| <span data-ttu-id="b6df2-135">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="b6df2-135">sharepointIds</span></span> | <span data-ttu-id="b6df2-136">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="b6df2-136">[sharepointIds][]</span></span> | <span data-ttu-id="b6df2-p106">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6df2-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>

[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares-get.md

## <a name="remarks"></a><span data-ttu-id="b6df2-142">Замечания</span><span class="sxs-lookup"><span data-stu-id="b6df2-142">Remarks</span></span>

<span data-ttu-id="b6df2-143">Чтобы обратиться к элементу **driveItem** из ресурса **itemReference**, составьте URL-адрес в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="b6df2-143">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="b6df2-144">Значение **path** — это путь к API относительно целевого диска, например: `/drive/root:/Documents/myfile.docx`.</span><span class="sxs-lookup"><span data-stu-id="b6df2-144">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="b6df2-145">Чтобы получить удобочитаемый путь для навигации, вы можете пропустить все до первого символа `:` в строке пути.</span><span class="sxs-lookup"><span data-stu-id="b6df2-145">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ItemReference returns a pointer to another item.",
  "section": "documentation",
  "tocPath": "Resources/ItemReference"
} -->
