---
title: Тип ресурса Воркбукворкшитпротектион
description: Представляет защиту объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ab5d3101b1b9cabf8843d3726f036de74bf3a258
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519101"
---
# <a name="workbookworksheetprotection-resource-type"></a><span data-ttu-id="e9a7e-103">Тип ресурса Воркбукворкшитпротектион</span><span class="sxs-lookup"><span data-stu-id="e9a7e-103">workbookWorksheetProtection resource type</span></span>

<span data-ttu-id="e9a7e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9a7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9a7e-105">Представляет защиту объекта листа.</span><span class="sxs-lookup"><span data-stu-id="e9a7e-105">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="e9a7e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e9a7e-106">Methods</span></span>

| <span data-ttu-id="e9a7e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e9a7e-107">Method</span></span>           | <span data-ttu-id="e9a7e-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e9a7e-108">Return Type</span></span>    |<span data-ttu-id="e9a7e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e9a7e-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e9a7e-110">Получение Воркбукворкшитпротектион</span><span class="sxs-lookup"><span data-stu-id="e9a7e-110">Get workbookWorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="e9a7e-111">воркбукворкшитпротектион</span><span class="sxs-lookup"><span data-stu-id="e9a7e-111">workbookWorksheetProtection</span></span>](workbookworksheetprotection.md) |<span data-ttu-id="e9a7e-112">Чтение свойств и связей объекта Воркбукворкшитпротектион.</span><span class="sxs-lookup"><span data-stu-id="e9a7e-112">Read properties and relationships of workbookWorksheetProtection object.</span></span>|
|[<span data-ttu-id="e9a7e-113">Protect</span><span class="sxs-lookup"><span data-stu-id="e9a7e-113">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="e9a7e-114">Нет</span><span class="sxs-lookup"><span data-stu-id="e9a7e-114">None</span></span>|<span data-ttu-id="e9a7e-p101">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="e9a7e-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="e9a7e-117">Unprotect</span><span class="sxs-lookup"><span data-stu-id="e9a7e-117">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="e9a7e-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e9a7e-118">None</span></span>|<span data-ttu-id="e9a7e-119">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="e9a7e-119">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="e9a7e-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9a7e-120">Properties</span></span>
| <span data-ttu-id="e9a7e-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9a7e-121">Property</span></span>     | <span data-ttu-id="e9a7e-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e9a7e-122">Type</span></span>   |<span data-ttu-id="e9a7e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e9a7e-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9a7e-124">options</span><span class="sxs-lookup"><span data-stu-id="e9a7e-124">options</span></span>|[<span data-ttu-id="e9a7e-125">воркбукворкшитпротектионоптионс</span><span class="sxs-lookup"><span data-stu-id="e9a7e-125">workbookWorksheetProtectionOptions</span></span>](workbookworksheetprotectionoptions.md)|<span data-ttu-id="e9a7e-126">Параметры защиты листа.</span><span class="sxs-lookup"><span data-stu-id="e9a7e-126">Sheet protection options.</span></span> <span data-ttu-id="e9a7e-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9a7e-127">Read-only.</span></span>|
|<span data-ttu-id="e9a7e-128">protected</span><span class="sxs-lookup"><span data-stu-id="e9a7e-128">protected</span></span>|<span data-ttu-id="e9a7e-129">boolean</span><span class="sxs-lookup"><span data-stu-id="e9a7e-129">boolean</span></span>|<span data-ttu-id="e9a7e-p103">Указывает, защищен ли лист.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9a7e-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9a7e-132">Связи</span><span class="sxs-lookup"><span data-stu-id="e9a7e-132">Relationships</span></span>
<span data-ttu-id="e9a7e-133">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e9a7e-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9a7e-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e9a7e-134">JSON representation</span></span>

<span data-ttu-id="e9a7e-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9a7e-135">Here is a JSON representation of the resource.</span></span>

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
