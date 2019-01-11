---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ItemReference
localization_priority: Normal
ms.openlocfilehash: 068e6420344cfa384972abe31157b3306f5b2a4f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862218"
---
# <a name="itemreference-resource-type"></a><span data-ttu-id="a7b0a-102">Тип ресурса ItemReference</span><span class="sxs-lookup"><span data-stu-id="a7b0a-102">ItemReference resource type</span></span>

<span data-ttu-id="a7b0a-103">Ресурс **ItemReference** предоставляет сведения, необходимые для обращения к ресурсу [DriveItem](driveitem.md) через API.</span><span class="sxs-lookup"><span data-stu-id="a7b0a-103">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7b0a-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7b0a-104">JSON representation</span></span>

<span data-ttu-id="a7b0a-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="a7b0a-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="a7b0a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7b0a-106">Properties</span></span>

| <span data-ttu-id="a7b0a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7b0a-107">Property</span></span>      | <span data-ttu-id="a7b0a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a7b0a-108">Type</span></span>              | <span data-ttu-id="a7b0a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a7b0a-109">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="a7b0a-110">driveId</span><span class="sxs-lookup"><span data-stu-id="a7b0a-110">driveId</span></span>       | <span data-ttu-id="a7b0a-111">String</span><span class="sxs-lookup"><span data-stu-id="a7b0a-111">String</span></span>            | <span data-ttu-id="a7b0a-p101">Уникальный идентификатор экземпляра диска, содержащего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a7b0a-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>
| <span data-ttu-id="a7b0a-114">driveType</span><span class="sxs-lookup"><span data-stu-id="a7b0a-114">driveType</span></span>     | <span data-ttu-id="a7b0a-115">String</span><span class="sxs-lookup"><span data-stu-id="a7b0a-115">String</span></span>            | <span data-ttu-id="a7b0a-116">Служит для идентификации типа для объекта drive.</span><span class="sxs-lookup"><span data-stu-id="a7b0a-116">Identifies the type of drive.</span></span> <span data-ttu-id="a7b0a-117">Сведения о возможных значениях см. в статье, посвященной ресурсу [drive][].</span><span class="sxs-lookup"><span data-stu-id="a7b0a-117">See [drive][] resource for values.</span></span>
| <span data-ttu-id="a7b0a-118">id</span><span class="sxs-lookup"><span data-stu-id="a7b0a-118">id</span></span>            | <span data-ttu-id="a7b0a-119">String</span><span class="sxs-lookup"><span data-stu-id="a7b0a-119">String</span></span>            | <span data-ttu-id="a7b0a-p103">Уникальный идентификатор элемента на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a7b0a-p103">Unique identifier of the item in the drive. Read-only.</span></span>
| <span data-ttu-id="a7b0a-122">name</span><span class="sxs-lookup"><span data-stu-id="a7b0a-122">name</span></span>          | <span data-ttu-id="a7b0a-123">Строка</span><span class="sxs-lookup"><span data-stu-id="a7b0a-123">String</span></span>            | <span data-ttu-id="a7b0a-p104">Имя элемента, на который направлена ссылка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a7b0a-p104">The name of the item being referenced. Read-only.</span></span>
| <span data-ttu-id="a7b0a-126">path</span><span class="sxs-lookup"><span data-stu-id="a7b0a-126">path</span></span>          | <span data-ttu-id="a7b0a-127">String</span><span class="sxs-lookup"><span data-stu-id="a7b0a-127">String</span></span>            | <span data-ttu-id="a7b0a-p105">Путь, по которому можно перейти к элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a7b0a-p105">Path that can be used to navigate to the item. Read-only.</span></span>
| <span data-ttu-id="a7b0a-130">shareId</span><span class="sxs-lookup"><span data-stu-id="a7b0a-130">shareId</span></span>       | <span data-ttu-id="a7b0a-131">String</span><span class="sxs-lookup"><span data-stu-id="a7b0a-131">String</span></span>            | <span data-ttu-id="a7b0a-132">Уникальный идентификатор общего ресурса, доступ к которому можно получить с помощью API [Shares][].</span><span class="sxs-lookup"><span data-stu-id="a7b0a-132">A unique identifier for a shared resource that can be accessed via the [Shares][] API.</span></span>
| <span data-ttu-id="a7b0a-133">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="a7b0a-133">sharepointIds</span></span> | <span data-ttu-id="a7b0a-134">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="a7b0a-134">[sharepointIds][]</span></span> | <span data-ttu-id="a7b0a-p106">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a7b0a-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>

[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares-get.md

## <a name="remarks"></a><span data-ttu-id="a7b0a-140">Замечания</span><span class="sxs-lookup"><span data-stu-id="a7b0a-140">Remarks</span></span>

<span data-ttu-id="a7b0a-141">Чтобы обратиться к элементу **driveItem** из ресурса **itemReference**, составьте URL-адрес в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="a7b0a-141">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="a7b0a-142">Значение **path** — это путь к API относительно целевого диска, например: `/drive/root:/Documents/myfile.docx`.</span><span class="sxs-lookup"><span data-stu-id="a7b0a-142">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="a7b0a-143">Чтобы получить удобочитаемый путь для навигации, вы можете пропустить все до первого символа `:` в строке пути.</span><span class="sxs-lookup"><span data-stu-id="a7b0a-143">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

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
