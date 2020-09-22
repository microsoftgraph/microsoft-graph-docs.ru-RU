---
title: Тип ресурса WorksheetProtection
description: Представляет защиту объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 8bb91dae367f9f9c95465aed0f8c71a26aaddd1a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015003"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="f067c-103">Тип ресурса WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="f067c-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="f067c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f067c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f067c-105">Представляет защиту объекта листа.</span><span class="sxs-lookup"><span data-stu-id="f067c-105">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="f067c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f067c-106">Methods</span></span>

| <span data-ttu-id="f067c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f067c-107">Method</span></span>           | <span data-ttu-id="f067c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f067c-108">Return Type</span></span>    |<span data-ttu-id="f067c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f067c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f067c-110">Получение объекта WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="f067c-110">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="f067c-111">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="f067c-111">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="f067c-112">Чтение свойств и связей объекта worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="f067c-112">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="f067c-113">Protect</span><span class="sxs-lookup"><span data-stu-id="f067c-113">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="f067c-114">Нет</span><span class="sxs-lookup"><span data-stu-id="f067c-114">None</span></span>|<span data-ttu-id="f067c-p101">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="f067c-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="f067c-117">Unprotect</span><span class="sxs-lookup"><span data-stu-id="f067c-117">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="f067c-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f067c-118">None</span></span>|<span data-ttu-id="f067c-119">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="f067c-119">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="f067c-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="f067c-120">Properties</span></span>
| <span data-ttu-id="f067c-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="f067c-121">Property</span></span>     | <span data-ttu-id="f067c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="f067c-122">Type</span></span>   |<span data-ttu-id="f067c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f067c-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f067c-124">options</span><span class="sxs-lookup"><span data-stu-id="f067c-124">options</span></span>|[<span data-ttu-id="f067c-125">воркбукворкшитпротектионоптионс</span><span class="sxs-lookup"><span data-stu-id="f067c-125">workbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="f067c-126">Параметры защиты листа.</span><span class="sxs-lookup"><span data-stu-id="f067c-126">Sheet protection options.</span></span> <span data-ttu-id="f067c-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f067c-127">Read-only.</span></span>|
|<span data-ttu-id="f067c-128">protected</span><span class="sxs-lookup"><span data-stu-id="f067c-128">protected</span></span>|<span data-ttu-id="f067c-129">boolean</span><span class="sxs-lookup"><span data-stu-id="f067c-129">boolean</span></span>|<span data-ttu-id="f067c-p103">Указывает, защищен ли лист.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f067c-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f067c-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f067c-132">JSON representation</span></span>

<span data-ttu-id="f067c-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f067c-133">Here is a JSON representation of the resource.</span></span>

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

