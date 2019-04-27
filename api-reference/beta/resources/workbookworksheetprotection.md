---
title: Тип ресурса Воркбукворкшитпротектион
description: Представляет защиту объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7e4a2f3130c71df35b1106d1a342004cfc6fdf25
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348958"
---
# <a name="workbookworksheetprotection-resource-type"></a><span data-ttu-id="4d2a2-103">Тип ресурса Воркбукворкшитпротектион</span><span class="sxs-lookup"><span data-stu-id="4d2a2-103">workbookWorksheetProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d2a2-104">Представляет защиту объекта листа.</span><span class="sxs-lookup"><span data-stu-id="4d2a2-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="4d2a2-105">Методы</span><span class="sxs-lookup"><span data-stu-id="4d2a2-105">Methods</span></span>

| <span data-ttu-id="4d2a2-106">Метод</span><span class="sxs-lookup"><span data-stu-id="4d2a2-106">Method</span></span>           | <span data-ttu-id="4d2a2-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4d2a2-107">Return Type</span></span>    |<span data-ttu-id="4d2a2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4d2a2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4d2a2-109">Получение Воркбукворкшитпротектион</span><span class="sxs-lookup"><span data-stu-id="4d2a2-109">Get workbookWorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="4d2a2-110">Воркбукворкшитпротектион</span><span class="sxs-lookup"><span data-stu-id="4d2a2-110">workbookWorksheetProtection</span></span>](workbookworksheetprotection.md) |<span data-ttu-id="4d2a2-111">Чтение свойств и связей объекта Воркбукворкшитпротектион.</span><span class="sxs-lookup"><span data-stu-id="4d2a2-111">Read properties and relationships of workbookWorksheetProtection object.</span></span>|
|[<span data-ttu-id="4d2a2-112">Protect</span><span class="sxs-lookup"><span data-stu-id="4d2a2-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="4d2a2-113">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="4d2a2-113">None</span></span>|<span data-ttu-id="4d2a2-p101">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="4d2a2-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="4d2a2-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="4d2a2-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="4d2a2-117">Нет</span><span class="sxs-lookup"><span data-stu-id="4d2a2-117">None</span></span>|<span data-ttu-id="4d2a2-118">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="4d2a2-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="4d2a2-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d2a2-119">Properties</span></span>
| <span data-ttu-id="4d2a2-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d2a2-120">Property</span></span>     | <span data-ttu-id="4d2a2-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4d2a2-121">Type</span></span>   |<span data-ttu-id="4d2a2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4d2a2-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d2a2-123">options</span><span class="sxs-lookup"><span data-stu-id="4d2a2-123">options</span></span>|[<span data-ttu-id="4d2a2-124">Воркбукворкшитпротектионоптионс</span><span class="sxs-lookup"><span data-stu-id="4d2a2-124">workbookWorksheetProtectionOptions</span></span>](workbookworksheetprotectionoptions.md)|<span data-ttu-id="4d2a2-125">Параметры защиты листа.</span><span class="sxs-lookup"><span data-stu-id="4d2a2-125">Sheet protection options.</span></span> <span data-ttu-id="4d2a2-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d2a2-126">Read-only.</span></span>|
|<span data-ttu-id="4d2a2-127">protected</span><span class="sxs-lookup"><span data-stu-id="4d2a2-127">protected</span></span>|<span data-ttu-id="4d2a2-128">boolean</span><span class="sxs-lookup"><span data-stu-id="4d2a2-128">boolean</span></span>|<span data-ttu-id="4d2a2-p103">Указывает, защищен ли лист.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d2a2-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d2a2-131">Связи</span><span class="sxs-lookup"><span data-stu-id="4d2a2-131">Relationships</span></span>
<span data-ttu-id="4d2a2-132">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4d2a2-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d2a2-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4d2a2-133">JSON representation</span></span>

<span data-ttu-id="4d2a2-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d2a2-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "options"
  ],
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": "boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookWorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
