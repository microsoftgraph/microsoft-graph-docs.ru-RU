---
title: Тип ресурса WorksheetProtection
description: Представляет защиту объекта листа.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: f0bbf3652223a532cd3d815aca832d4cfcd37171
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860715"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="1fe88-103">Тип ресурса WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="1fe88-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="1fe88-104">Представляет защиту объекта листа.</span><span class="sxs-lookup"><span data-stu-id="1fe88-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="1fe88-105">Методы</span><span class="sxs-lookup"><span data-stu-id="1fe88-105">Methods</span></span>

| <span data-ttu-id="1fe88-106">Метод</span><span class="sxs-lookup"><span data-stu-id="1fe88-106">Method</span></span>           | <span data-ttu-id="1fe88-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1fe88-107">Return Type</span></span>    |<span data-ttu-id="1fe88-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1fe88-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1fe88-109">Получение объекта WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="1fe88-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="1fe88-110">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="1fe88-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="1fe88-111">Чтение свойств и связей объекта worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="1fe88-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="1fe88-112">Protect</span><span class="sxs-lookup"><span data-stu-id="1fe88-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="1fe88-113">Нет</span><span class="sxs-lookup"><span data-stu-id="1fe88-113">None</span></span>|<span data-ttu-id="1fe88-p101">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="1fe88-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="1fe88-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="1fe88-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="1fe88-117">Нет</span><span class="sxs-lookup"><span data-stu-id="1fe88-117">None</span></span>|<span data-ttu-id="1fe88-118">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="1fe88-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="1fe88-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="1fe88-119">Properties</span></span>
| <span data-ttu-id="1fe88-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="1fe88-120">Property</span></span>     | <span data-ttu-id="1fe88-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1fe88-121">Type</span></span>   |<span data-ttu-id="1fe88-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1fe88-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1fe88-123">options</span><span class="sxs-lookup"><span data-stu-id="1fe88-123">options</span></span>|[<span data-ttu-id="1fe88-124">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="1fe88-124">WorkbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="1fe88-p102">Параметры защиты листа. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1fe88-p102">Sheet protection options. Read-only.</span></span>|
|<span data-ttu-id="1fe88-127">protected</span><span class="sxs-lookup"><span data-stu-id="1fe88-127">protected</span></span>|<span data-ttu-id="1fe88-128">boolean</span><span class="sxs-lookup"><span data-stu-id="1fe88-128">boolean</span></span>|<span data-ttu-id="1fe88-p103">Указывает, защищен ли лист.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1fe88-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1fe88-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1fe88-131">JSON representation</span></span>

<span data-ttu-id="1fe88-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1fe88-132">Here is a JSON representation of the resource.</span></span>

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
