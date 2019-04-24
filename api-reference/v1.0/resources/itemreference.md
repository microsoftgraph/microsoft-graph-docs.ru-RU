---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ItemReference
localization_priority: Normal
ms.openlocfilehash: 5c60ee4a0ac8538d71d37403e6f790e32d6a74cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585225"
---
# <a name="itemreference-resource-type"></a><span data-ttu-id="477cc-102">Тип ресурса ItemReference</span><span class="sxs-lookup"><span data-stu-id="477cc-102">ItemReference resource type</span></span>

<span data-ttu-id="477cc-103">Ресурс **ItemReference** предоставляет сведения, необходимые для обращения к ресурсу [DriveItem](driveitem.md) через API.</span><span class="sxs-lookup"><span data-stu-id="477cc-103">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="477cc-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="477cc-104">JSON representation</span></span>

<span data-ttu-id="477cc-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="477cc-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="477cc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="477cc-106">Properties</span></span>

| <span data-ttu-id="477cc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="477cc-107">Property</span></span>      | <span data-ttu-id="477cc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="477cc-108">Type</span></span>              | <span data-ttu-id="477cc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="477cc-109">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="477cc-110">driveId</span><span class="sxs-lookup"><span data-stu-id="477cc-110">driveId</span></span>       | <span data-ttu-id="477cc-111">Строка</span><span class="sxs-lookup"><span data-stu-id="477cc-111">String</span></span>            | <span data-ttu-id="477cc-p101">Уникальный идентификатор экземпляра диска, содержащего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="477cc-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>
| <span data-ttu-id="477cc-114">driveType</span><span class="sxs-lookup"><span data-stu-id="477cc-114">driveType</span></span>     | <span data-ttu-id="477cc-115">String</span><span class="sxs-lookup"><span data-stu-id="477cc-115">String</span></span>            | <span data-ttu-id="477cc-116">Служит для идентификации типа для объекта drive.</span><span class="sxs-lookup"><span data-stu-id="477cc-116">Identifies the type of drive.</span></span> <span data-ttu-id="477cc-117">Сведения о возможных значениях см. в статье, посвященной ресурсу [drive][].</span><span class="sxs-lookup"><span data-stu-id="477cc-117">See [drive][] resource for values.</span></span>
| <span data-ttu-id="477cc-118">id</span><span class="sxs-lookup"><span data-stu-id="477cc-118">id</span></span>            | <span data-ttu-id="477cc-119">String</span><span class="sxs-lookup"><span data-stu-id="477cc-119">String</span></span>            | <span data-ttu-id="477cc-p103">Уникальный идентификатор элемента на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="477cc-p103">Unique identifier of the item in the drive. Read-only.</span></span>
| <span data-ttu-id="477cc-122">name</span><span class="sxs-lookup"><span data-stu-id="477cc-122">name</span></span>          | <span data-ttu-id="477cc-123">String</span><span class="sxs-lookup"><span data-stu-id="477cc-123">String</span></span>            | <span data-ttu-id="477cc-p104">Имя элемента, на который направлена ссылка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="477cc-p104">The name of the item being referenced. Read-only.</span></span>
| <span data-ttu-id="477cc-126">path</span><span class="sxs-lookup"><span data-stu-id="477cc-126">path</span></span>          | <span data-ttu-id="477cc-127">String</span><span class="sxs-lookup"><span data-stu-id="477cc-127">String</span></span>            | <span data-ttu-id="477cc-p105">Путь, по которому можно перейти к элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="477cc-p105">Path that can be used to navigate to the item. Read-only.</span></span>
| <span data-ttu-id="477cc-130">shareId</span><span class="sxs-lookup"><span data-stu-id="477cc-130">shareId</span></span>       | <span data-ttu-id="477cc-131">Строка</span><span class="sxs-lookup"><span data-stu-id="477cc-131">String</span></span>            | <span data-ttu-id="477cc-132">Уникальный идентификатор общего ресурса, доступ к которому можно получить с помощью API [Shares][].</span><span class="sxs-lookup"><span data-stu-id="477cc-132">A unique identifier for a shared resource that can be accessed via the [Shares][] API.</span></span>
| <span data-ttu-id="477cc-133">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="477cc-133">sharepointIds</span></span> | <span data-ttu-id="477cc-134">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="477cc-134">[sharepointIds][]</span></span> | <span data-ttu-id="477cc-p106">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="477cc-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>

[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares-get.md

## <a name="remarks"></a><span data-ttu-id="477cc-140">Замечания</span><span class="sxs-lookup"><span data-stu-id="477cc-140">Remarks</span></span>

<span data-ttu-id="477cc-141">Чтобы обратиться к элементу **driveItem** из ресурса **itemReference**, составьте URL-адрес в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="477cc-141">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="477cc-142">Значение **path** — это путь к API относительно целевого диска, например: `/drive/root:/Documents/myfile.docx`.</span><span class="sxs-lookup"><span data-stu-id="477cc-142">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="477cc-143">Чтобы получить удобочитаемый путь для навигации, вы можете пропустить все до первого символа `:` в строке пути.</span><span class="sxs-lookup"><span data-stu-id="477cc-143">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

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
