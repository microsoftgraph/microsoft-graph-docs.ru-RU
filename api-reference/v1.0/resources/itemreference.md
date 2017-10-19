---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ItemReference
ms.openlocfilehash: abd8b438e6c4e364a7a4b010d0808255425fa4df
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="itemreference-resource-type"></a><span data-ttu-id="59e39-102">Тип ресурса ItemReference</span><span class="sxs-lookup"><span data-stu-id="59e39-102">ItemReference resource type</span></span>

<span data-ttu-id="59e39-103">Ресурс **ItemReference** предоставляет сведения, необходимые для обращения к ресурсу [DriveItem](driveitem.md) через API.</span><span class="sxs-lookup"><span data-stu-id="59e39-103">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="59e39-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59e39-104">JSON representation</span></span>

<span data-ttu-id="59e39-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="59e39-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="59e39-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="59e39-106">Properties</span></span>

| <span data-ttu-id="59e39-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="59e39-107">Property</span></span>      | <span data-ttu-id="59e39-108">Тип</span><span class="sxs-lookup"><span data-stu-id="59e39-108">Type</span></span>              | <span data-ttu-id="59e39-109">Описание</span><span class="sxs-lookup"><span data-stu-id="59e39-109">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="59e39-110">driveId</span><span class="sxs-lookup"><span data-stu-id="59e39-110">driveId</span></span>       | <span data-ttu-id="59e39-111">String</span><span class="sxs-lookup"><span data-stu-id="59e39-111">String</span></span>            | <span data-ttu-id="59e39-p101">Уникальный идентификатор экземпляра диска, содержащего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="59e39-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>
| <span data-ttu-id="59e39-114">driveType</span><span class="sxs-lookup"><span data-stu-id="59e39-114">driveType</span></span>     | <span data-ttu-id="59e39-115">String</span><span class="sxs-lookup"><span data-stu-id="59e39-115">String</span></span>            | <span data-ttu-id="59e39-116">Служит для идентификации типа диска.</span><span class="sxs-lookup"><span data-stu-id="59e39-116">Identifies the type of drive.</span></span> <span data-ttu-id="59e39-117">Сведения о возможных значениях см. в статье, посвященной ресурсу [drive][].</span><span class="sxs-lookup"><span data-stu-id="59e39-117">See [drive][] resource for values.</span></span>
| <span data-ttu-id="59e39-118">id</span><span class="sxs-lookup"><span data-stu-id="59e39-118">id</span></span>            | <span data-ttu-id="59e39-119">String</span><span class="sxs-lookup"><span data-stu-id="59e39-119">String</span></span>            | <span data-ttu-id="59e39-p103">Уникальный идентификатор элемента на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="59e39-p103">Unique identifier of the item in the drive. Read-only.</span></span>
| <span data-ttu-id="59e39-122">name</span><span class="sxs-lookup"><span data-stu-id="59e39-122">name</span></span>          | <span data-ttu-id="59e39-123">Строка</span><span class="sxs-lookup"><span data-stu-id="59e39-123">String</span></span>            | <span data-ttu-id="59e39-p104">Имя элемента, на который направлена ссылка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="59e39-p104">The name of the item being referenced. Read-only.</span></span>
| <span data-ttu-id="59e39-126">path</span><span class="sxs-lookup"><span data-stu-id="59e39-126">path</span></span>          | <span data-ttu-id="59e39-127">String</span><span class="sxs-lookup"><span data-stu-id="59e39-127">String</span></span>            | <span data-ttu-id="59e39-p105">Путь, по которому можно перейти к элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="59e39-p105">Path that can be used to navigate to the item. Read-only.</span></span>
| <span data-ttu-id="59e39-130">shareId</span><span class="sxs-lookup"><span data-stu-id="59e39-130">shareId</span></span>       | <span data-ttu-id="59e39-131">String</span><span class="sxs-lookup"><span data-stu-id="59e39-131">String</span></span>            | <span data-ttu-id="59e39-132">Уникальный идентификатор общего ресурса, доступ к которому можно получить с помощью API [Shares][].</span><span class="sxs-lookup"><span data-stu-id="59e39-132">A unique identifier for a shared resource that can be accessed via the [Shares][] API.</span></span>
| <span data-ttu-id="59e39-133">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="59e39-133">sharepointIds</span></span> | <span data-ttu-id="59e39-134">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="59e39-134">[sharepointIds][]</span></span> | <span data-ttu-id="59e39-p106">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="59e39-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>

[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares_get.md

## <a name="remarks"></a><span data-ttu-id="59e39-140">Примечания</span><span class="sxs-lookup"><span data-stu-id="59e39-140">Remarks</span></span>

<span data-ttu-id="59e39-141">Чтобы обратиться к элементу **driveItem** из ресурса **itemReference**, составьте URL-адрес в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="59e39-141">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="59e39-142">Значение **path** — это путь к API относительно целевого диска, например: `/drive/root:/Documents/myfile.docx`.</span><span class="sxs-lookup"><span data-stu-id="59e39-142">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="59e39-143">Чтобы получить удобочитаемый путь для навигации, вы можете пропустить все до первого символа `:` в строке пути.</span><span class="sxs-lookup"><span data-stu-id="59e39-143">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ItemReference returns a pointer to another item.",
  "section": "documentation",
  "tocPath": "Resources/ItemReference"
} -->
