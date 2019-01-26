---
title: Тип ресурса WorksheetProtection
description: Представляет защиту объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6f32ad7b1cc25d9a937f2de68f1bd930d92ec8f9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572936"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="7a752-103">Тип ресурса WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="7a752-103">WorksheetProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a752-104">Представляет защиту объекта листа.</span><span class="sxs-lookup"><span data-stu-id="7a752-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="7a752-105">Методы</span><span class="sxs-lookup"><span data-stu-id="7a752-105">Methods</span></span>

| <span data-ttu-id="7a752-106">Метод</span><span class="sxs-lookup"><span data-stu-id="7a752-106">Method</span></span>           | <span data-ttu-id="7a752-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7a752-107">Return Type</span></span>    |<span data-ttu-id="7a752-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7a752-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7a752-109">Получение объекта WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="7a752-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="7a752-110">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="7a752-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="7a752-111">Чтение свойств и связей объекта worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="7a752-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="7a752-112">Protect</span><span class="sxs-lookup"><span data-stu-id="7a752-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="7a752-113">Нет</span><span class="sxs-lookup"><span data-stu-id="7a752-113">None</span></span>|<span data-ttu-id="7a752-p101">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="7a752-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="7a752-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="7a752-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="7a752-117">Нет</span><span class="sxs-lookup"><span data-stu-id="7a752-117">None</span></span>|<span data-ttu-id="7a752-118">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="7a752-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="7a752-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a752-119">Properties</span></span>
| <span data-ttu-id="7a752-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a752-120">Property</span></span>     | <span data-ttu-id="7a752-121">Тип</span><span class="sxs-lookup"><span data-stu-id="7a752-121">Type</span></span>   |<span data-ttu-id="7a752-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7a752-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a752-123">protected</span><span class="sxs-lookup"><span data-stu-id="7a752-123">protected</span></span>|<span data-ttu-id="7a752-124">boolean</span><span class="sxs-lookup"><span data-stu-id="7a752-124">boolean</span></span>|<span data-ttu-id="7a752-p102">Указывает, защищен ли лист.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a752-p102">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a752-127">Связи</span><span class="sxs-lookup"><span data-stu-id="7a752-127">Relationships</span></span>
| <span data-ttu-id="7a752-128">Связь</span><span class="sxs-lookup"><span data-stu-id="7a752-128">Relationship</span></span> | <span data-ttu-id="7a752-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7a752-129">Type</span></span>   |<span data-ttu-id="7a752-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7a752-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a752-131">options</span><span class="sxs-lookup"><span data-stu-id="7a752-131">options</span></span>|[<span data-ttu-id="7a752-132">workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="7a752-132">workbookWorksheetProtection</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="7a752-p103">Параметры защиты листа. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a752-p103">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a752-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a752-135">JSON representation</span></span>

<span data-ttu-id="7a752-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a752-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "options"
  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/worksheetprotection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
