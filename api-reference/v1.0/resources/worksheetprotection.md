---
title: Тип ресурса WorksheetProtection
description: Представляет защиту объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c8a719d1be9f21edf1bef82d2aa058b45bbf2df8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984236"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="51d27-103">Тип ресурса WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="51d27-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="51d27-104">Представляет защиту объекта листа.</span><span class="sxs-lookup"><span data-stu-id="51d27-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="51d27-105">Методы</span><span class="sxs-lookup"><span data-stu-id="51d27-105">Methods</span></span>

| <span data-ttu-id="51d27-106">Метод</span><span class="sxs-lookup"><span data-stu-id="51d27-106">Method</span></span>           | <span data-ttu-id="51d27-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="51d27-107">Return Type</span></span>    |<span data-ttu-id="51d27-108">Описание</span><span class="sxs-lookup"><span data-stu-id="51d27-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="51d27-109">Получение объекта WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="51d27-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="51d27-110">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="51d27-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="51d27-111">Чтение свойств и связей объекта worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="51d27-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="51d27-112">Protect</span><span class="sxs-lookup"><span data-stu-id="51d27-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="51d27-113">Нет</span><span class="sxs-lookup"><span data-stu-id="51d27-113">None</span></span>|<span data-ttu-id="51d27-p101">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="51d27-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="51d27-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="51d27-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="51d27-117">Нет</span><span class="sxs-lookup"><span data-stu-id="51d27-117">None</span></span>|<span data-ttu-id="51d27-118">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="51d27-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="51d27-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="51d27-119">Properties</span></span>
| <span data-ttu-id="51d27-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="51d27-120">Property</span></span>     | <span data-ttu-id="51d27-121">Тип</span><span class="sxs-lookup"><span data-stu-id="51d27-121">Type</span></span>   |<span data-ttu-id="51d27-122">Описание</span><span class="sxs-lookup"><span data-stu-id="51d27-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51d27-123">options</span><span class="sxs-lookup"><span data-stu-id="51d27-123">options</span></span>|[<span data-ttu-id="51d27-124">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="51d27-124">WorkbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="51d27-p102">Параметры защиты листа. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="51d27-p102">Sheet protection options. Read-only.</span></span>|
|<span data-ttu-id="51d27-127">protected</span><span class="sxs-lookup"><span data-stu-id="51d27-127">protected</span></span>|<span data-ttu-id="51d27-128">boolean</span><span class="sxs-lookup"><span data-stu-id="51d27-128">boolean</span></span>|<span data-ttu-id="51d27-p103">Указывает, защищен ли лист.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="51d27-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51d27-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51d27-131">JSON representation</span></span>

<span data-ttu-id="51d27-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51d27-132">Here is a JSON representation of the resource.</span></span>

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
