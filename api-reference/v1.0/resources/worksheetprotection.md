---
title: Тип ресурса WorksheetProtection
description: Представляет защиту объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c8a719d1be9f21edf1bef82d2aa058b45bbf2df8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463616"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="1b3ce-103">Тип ресурса WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="1b3ce-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="1b3ce-104">Представляет защиту объекта листа.</span><span class="sxs-lookup"><span data-stu-id="1b3ce-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="1b3ce-105">Методы</span><span class="sxs-lookup"><span data-stu-id="1b3ce-105">Methods</span></span>

| <span data-ttu-id="1b3ce-106">Метод</span><span class="sxs-lookup"><span data-stu-id="1b3ce-106">Method</span></span>           | <span data-ttu-id="1b3ce-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1b3ce-107">Return Type</span></span>    |<span data-ttu-id="1b3ce-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1b3ce-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1b3ce-109">Получение объекта WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="1b3ce-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="1b3ce-110">Воркбукворкшитпротектион</span><span class="sxs-lookup"><span data-stu-id="1b3ce-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="1b3ce-111">Чтение свойств и связей объекта worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="1b3ce-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="1b3ce-112">Protect</span><span class="sxs-lookup"><span data-stu-id="1b3ce-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="1b3ce-113">Нет</span><span class="sxs-lookup"><span data-stu-id="1b3ce-113">None</span></span>|<span data-ttu-id="1b3ce-p101">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="1b3ce-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="1b3ce-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="1b3ce-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="1b3ce-117">Нет</span><span class="sxs-lookup"><span data-stu-id="1b3ce-117">None</span></span>|<span data-ttu-id="1b3ce-118">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="1b3ce-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="1b3ce-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b3ce-119">Properties</span></span>
| <span data-ttu-id="1b3ce-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b3ce-120">Property</span></span>     | <span data-ttu-id="1b3ce-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1b3ce-121">Type</span></span>   |<span data-ttu-id="1b3ce-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1b3ce-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b3ce-123">options</span><span class="sxs-lookup"><span data-stu-id="1b3ce-123">options</span></span>|[<span data-ttu-id="1b3ce-124">Воркбукворкшитпротектионоптионс</span><span class="sxs-lookup"><span data-stu-id="1b3ce-124">WorkbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="1b3ce-125">Параметры защиты листа.</span><span class="sxs-lookup"><span data-stu-id="1b3ce-125">Sheet protection options.</span></span> <span data-ttu-id="1b3ce-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b3ce-126">Read-only.</span></span>|
|<span data-ttu-id="1b3ce-127">protected</span><span class="sxs-lookup"><span data-stu-id="1b3ce-127">protected</span></span>|<span data-ttu-id="1b3ce-128">boolean</span><span class="sxs-lookup"><span data-stu-id="1b3ce-128">boolean</span></span>|<span data-ttu-id="1b3ce-p103">Указывает, защищен ли лист.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b3ce-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b3ce-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b3ce-131">JSON representation</span></span>

<span data-ttu-id="1b3ce-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b3ce-132">Here is a JSON representation of the resource.</span></span>

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
