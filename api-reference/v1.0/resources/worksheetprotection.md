---
title: Тип ресурса WorksheetProtection
description: Представляет защиту объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1c92c02b9c5e2409ad3036bbc34c41588161ae79
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345402"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="55fc2-103">Тип ресурса WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="55fc2-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="55fc2-104">Представляет защиту объекта листа.</span><span class="sxs-lookup"><span data-stu-id="55fc2-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="55fc2-105">Методы</span><span class="sxs-lookup"><span data-stu-id="55fc2-105">Methods</span></span>

| <span data-ttu-id="55fc2-106">Метод</span><span class="sxs-lookup"><span data-stu-id="55fc2-106">Method</span></span>           | <span data-ttu-id="55fc2-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="55fc2-107">Return Type</span></span>    |<span data-ttu-id="55fc2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="55fc2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="55fc2-109">Получение объекта WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="55fc2-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="55fc2-110">Воркбукворкшитпротектион</span><span class="sxs-lookup"><span data-stu-id="55fc2-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="55fc2-111">Чтение свойств и связей объекта worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="55fc2-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="55fc2-112">Protect</span><span class="sxs-lookup"><span data-stu-id="55fc2-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="55fc2-113">Нет</span><span class="sxs-lookup"><span data-stu-id="55fc2-113">None</span></span>|<span data-ttu-id="55fc2-p101">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="55fc2-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="55fc2-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="55fc2-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="55fc2-117">Нет</span><span class="sxs-lookup"><span data-stu-id="55fc2-117">None</span></span>|<span data-ttu-id="55fc2-118">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="55fc2-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="55fc2-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="55fc2-119">Properties</span></span>
| <span data-ttu-id="55fc2-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="55fc2-120">Property</span></span>     | <span data-ttu-id="55fc2-121">Тип</span><span class="sxs-lookup"><span data-stu-id="55fc2-121">Type</span></span>   |<span data-ttu-id="55fc2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="55fc2-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55fc2-123">options</span><span class="sxs-lookup"><span data-stu-id="55fc2-123">options</span></span>|[<span data-ttu-id="55fc2-124">Воркбукворкшитпротектионоптионс</span><span class="sxs-lookup"><span data-stu-id="55fc2-124">workbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="55fc2-125">Параметры защиты листа.</span><span class="sxs-lookup"><span data-stu-id="55fc2-125">Sheet protection options.</span></span> <span data-ttu-id="55fc2-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55fc2-126">Read-only.</span></span>|
|<span data-ttu-id="55fc2-127">protected</span><span class="sxs-lookup"><span data-stu-id="55fc2-127">protected</span></span>|<span data-ttu-id="55fc2-128">boolean</span><span class="sxs-lookup"><span data-stu-id="55fc2-128">boolean</span></span>|<span data-ttu-id="55fc2-p103">Указывает, защищен ли лист.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55fc2-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55fc2-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="55fc2-131">JSON representation</span></span>

<span data-ttu-id="55fc2-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55fc2-132">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": true,
  "options": { "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
