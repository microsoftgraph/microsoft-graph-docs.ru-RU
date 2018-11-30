---
title: Тип ресурса WorksheetProtection
description: Представляет защиту объекта листа.
ms.openlocfilehash: aae92566503ce7bdb4a742c33b1a65c43937662c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025984"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="932e3-103">Тип ресурса WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="932e3-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="932e3-104">Представляет защиту объекта листа.</span><span class="sxs-lookup"><span data-stu-id="932e3-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="932e3-105">Методы</span><span class="sxs-lookup"><span data-stu-id="932e3-105">Methods</span></span>

| <span data-ttu-id="932e3-106">Метод</span><span class="sxs-lookup"><span data-stu-id="932e3-106">Method</span></span>           | <span data-ttu-id="932e3-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="932e3-107">Return Type</span></span>    |<span data-ttu-id="932e3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="932e3-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="932e3-109">Получение объекта WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="932e3-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="932e3-110">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="932e3-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="932e3-111">Чтение свойств и связей объекта worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="932e3-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="932e3-112">Protect</span><span class="sxs-lookup"><span data-stu-id="932e3-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="932e3-113">Нет</span><span class="sxs-lookup"><span data-stu-id="932e3-113">None</span></span>|<span data-ttu-id="932e3-p101">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="932e3-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="932e3-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="932e3-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="932e3-117">Нет</span><span class="sxs-lookup"><span data-stu-id="932e3-117">None</span></span>|<span data-ttu-id="932e3-118">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="932e3-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="932e3-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="932e3-119">Properties</span></span>
| <span data-ttu-id="932e3-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="932e3-120">Property</span></span>     | <span data-ttu-id="932e3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="932e3-121">Type</span></span>   |<span data-ttu-id="932e3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="932e3-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="932e3-123">options</span><span class="sxs-lookup"><span data-stu-id="932e3-123">options</span></span>|[<span data-ttu-id="932e3-124">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="932e3-124">WorkbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="932e3-p102">Параметры защиты листа. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="932e3-p102">Sheet protection options. Read-only.</span></span>|
|<span data-ttu-id="932e3-127">protected</span><span class="sxs-lookup"><span data-stu-id="932e3-127">protected</span></span>|<span data-ttu-id="932e3-128">boolean</span><span class="sxs-lookup"><span data-stu-id="932e3-128">boolean</span></span>|<span data-ttu-id="932e3-p103">Указывает, защищен ли лист.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="932e3-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="932e3-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="932e3-131">JSON representation</span></span>

<span data-ttu-id="932e3-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="932e3-132">Here is a JSON representation of the resource.</span></span>

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