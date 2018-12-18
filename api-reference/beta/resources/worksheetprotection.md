---
title: Тип ресурса WorksheetProtection
description: Представляет защиту объекта листа.
author: lumine2008
ms.openlocfilehash: 91415b067fbe54333e32d1a2ed84bce5025b7d3a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339209"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="8dfbc-103">Тип ресурса WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="8dfbc-103">WorksheetProtection resource type</span></span>

> <span data-ttu-id="8dfbc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8dfbc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8dfbc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dfbc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8dfbc-106">Представляет защиту объекта листа.</span><span class="sxs-lookup"><span data-stu-id="8dfbc-106">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="8dfbc-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8dfbc-107">Methods</span></span>

| <span data-ttu-id="8dfbc-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8dfbc-108">Method</span></span>           | <span data-ttu-id="8dfbc-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8dfbc-109">Return Type</span></span>    |<span data-ttu-id="8dfbc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8dfbc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8dfbc-111">Получение объекта WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="8dfbc-111">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="8dfbc-112">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="8dfbc-112">WorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="8dfbc-113">Чтение свойств и связей объекта worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="8dfbc-113">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="8dfbc-114">Protect</span><span class="sxs-lookup"><span data-stu-id="8dfbc-114">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="8dfbc-115">Нет</span><span class="sxs-lookup"><span data-stu-id="8dfbc-115">None</span></span>|<span data-ttu-id="8dfbc-p102">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="8dfbc-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="8dfbc-118">Unprotect</span><span class="sxs-lookup"><span data-stu-id="8dfbc-118">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="8dfbc-119">Нет</span><span class="sxs-lookup"><span data-stu-id="8dfbc-119">None</span></span>|<span data-ttu-id="8dfbc-120">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="8dfbc-120">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="8dfbc-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="8dfbc-121">Properties</span></span>
| <span data-ttu-id="8dfbc-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="8dfbc-122">Property</span></span>     | <span data-ttu-id="8dfbc-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8dfbc-123">Type</span></span>   |<span data-ttu-id="8dfbc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8dfbc-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8dfbc-125">protected</span><span class="sxs-lookup"><span data-stu-id="8dfbc-125">protected</span></span>|<span data-ttu-id="8dfbc-126">boolean</span><span class="sxs-lookup"><span data-stu-id="8dfbc-126">boolean</span></span>|<span data-ttu-id="8dfbc-p103">Указывает, защищен ли лист.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8dfbc-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8dfbc-129">Связи</span><span class="sxs-lookup"><span data-stu-id="8dfbc-129">Relationships</span></span>
| <span data-ttu-id="8dfbc-130">Связь</span><span class="sxs-lookup"><span data-stu-id="8dfbc-130">Relationship</span></span> | <span data-ttu-id="8dfbc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8dfbc-131">Type</span></span>   |<span data-ttu-id="8dfbc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8dfbc-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8dfbc-133">options</span><span class="sxs-lookup"><span data-stu-id="8dfbc-133">options</span></span>|[<span data-ttu-id="8dfbc-134">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="8dfbc-134">WorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="8dfbc-p104">Параметры защиты листа. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8dfbc-p104">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8dfbc-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8dfbc-137">JSON representation</span></span>

<span data-ttu-id="8dfbc-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8dfbc-138">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->