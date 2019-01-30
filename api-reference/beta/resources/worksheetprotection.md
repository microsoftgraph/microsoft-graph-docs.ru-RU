---
title: Тип ресурса WorksheetProtection
description: Представляет защиту объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7e87edcebae95f32ce0bccaf849a7d21140f4878
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29639946"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="4c4ce-103">Тип ресурса WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="4c4ce-103">WorksheetProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c4ce-104">Представляет защиту объекта листа.</span><span class="sxs-lookup"><span data-stu-id="4c4ce-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="4c4ce-105">Методы</span><span class="sxs-lookup"><span data-stu-id="4c4ce-105">Methods</span></span>

| <span data-ttu-id="4c4ce-106">Метод</span><span class="sxs-lookup"><span data-stu-id="4c4ce-106">Method</span></span>           | <span data-ttu-id="4c4ce-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4c4ce-107">Return Type</span></span>    |<span data-ttu-id="4c4ce-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4c4ce-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4c4ce-109">Получение объекта WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="4c4ce-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="4c4ce-110">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="4c4ce-110">WorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="4c4ce-111">Чтение свойств и связей объекта worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="4c4ce-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="4c4ce-112">Protect</span><span class="sxs-lookup"><span data-stu-id="4c4ce-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="4c4ce-113">Нет</span><span class="sxs-lookup"><span data-stu-id="4c4ce-113">None</span></span>|<span data-ttu-id="4c4ce-p101">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="4c4ce-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="4c4ce-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="4c4ce-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="4c4ce-117">Нет</span><span class="sxs-lookup"><span data-stu-id="4c4ce-117">None</span></span>|<span data-ttu-id="4c4ce-118">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="4c4ce-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="4c4ce-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c4ce-119">Properties</span></span>
| <span data-ttu-id="4c4ce-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c4ce-120">Property</span></span>     | <span data-ttu-id="4c4ce-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4c4ce-121">Type</span></span>   |<span data-ttu-id="4c4ce-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4c4ce-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c4ce-123">protected</span><span class="sxs-lookup"><span data-stu-id="4c4ce-123">protected</span></span>|<span data-ttu-id="4c4ce-124">boolean</span><span class="sxs-lookup"><span data-stu-id="4c4ce-124">boolean</span></span>|<span data-ttu-id="4c4ce-p102">Указывает, защищен ли лист.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4c4ce-p102">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c4ce-127">Связи</span><span class="sxs-lookup"><span data-stu-id="4c4ce-127">Relationships</span></span>
| <span data-ttu-id="4c4ce-128">Связь</span><span class="sxs-lookup"><span data-stu-id="4c4ce-128">Relationship</span></span> | <span data-ttu-id="4c4ce-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4c4ce-129">Type</span></span>   |<span data-ttu-id="4c4ce-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4c4ce-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c4ce-131">options</span><span class="sxs-lookup"><span data-stu-id="4c4ce-131">options</span></span>|[<span data-ttu-id="4c4ce-132">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="4c4ce-132">WorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="4c4ce-p103">Параметры защиты листа. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4c4ce-p103">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4c4ce-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c4ce-135">JSON representation</span></span>

<span data-ttu-id="4c4ce-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c4ce-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheetProtection"
}-->

```json
{
  "protected": true
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
