---
title: Тип ресурса WorksheetProtection
description: Представляет защиту объекта листа.
ms.openlocfilehash: 8886117df669201a0c8a6f9fda1df18bb47cc4a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082102"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="cd852-103">Тип ресурса WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="cd852-103">WorksheetProtection resource type</span></span>

> <span data-ttu-id="cd852-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cd852-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd852-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd852-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd852-106">Представляет защиту объекта листа.</span><span class="sxs-lookup"><span data-stu-id="cd852-106">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="cd852-107">Методы</span><span class="sxs-lookup"><span data-stu-id="cd852-107">Methods</span></span>

| <span data-ttu-id="cd852-108">Метод</span><span class="sxs-lookup"><span data-stu-id="cd852-108">Method</span></span>           | <span data-ttu-id="cd852-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cd852-109">Return Type</span></span>    |<span data-ttu-id="cd852-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cd852-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cd852-111">Получение объекта WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="cd852-111">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="cd852-112">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="cd852-112">WorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="cd852-113">Чтение свойств и связей объекта worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="cd852-113">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="cd852-114">Protect</span><span class="sxs-lookup"><span data-stu-id="cd852-114">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="cd852-115">Нет</span><span class="sxs-lookup"><span data-stu-id="cd852-115">None</span></span>|<span data-ttu-id="cd852-p102">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="cd852-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="cd852-118">Unprotect</span><span class="sxs-lookup"><span data-stu-id="cd852-118">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="cd852-119">Нет</span><span class="sxs-lookup"><span data-stu-id="cd852-119">None</span></span>|<span data-ttu-id="cd852-120">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="cd852-120">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="cd852-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd852-121">Properties</span></span>
| <span data-ttu-id="cd852-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd852-122">Property</span></span>     | <span data-ttu-id="cd852-123">Тип</span><span class="sxs-lookup"><span data-stu-id="cd852-123">Type</span></span>   |<span data-ttu-id="cd852-124">Описание</span><span class="sxs-lookup"><span data-stu-id="cd852-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd852-125">protected</span><span class="sxs-lookup"><span data-stu-id="cd852-125">protected</span></span>|<span data-ttu-id="cd852-126">boolean</span><span class="sxs-lookup"><span data-stu-id="cd852-126">boolean</span></span>|<span data-ttu-id="cd852-p103">Указывает, защищен ли лист.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd852-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd852-129">Связи</span><span class="sxs-lookup"><span data-stu-id="cd852-129">Relationships</span></span>
| <span data-ttu-id="cd852-130">Связь</span><span class="sxs-lookup"><span data-stu-id="cd852-130">Relationship</span></span> | <span data-ttu-id="cd852-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cd852-131">Type</span></span>   |<span data-ttu-id="cd852-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cd852-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd852-133">options</span><span class="sxs-lookup"><span data-stu-id="cd852-133">options</span></span>|[<span data-ttu-id="cd852-134">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="cd852-134">WorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="cd852-p104">Параметры защиты листа. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd852-p104">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd852-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd852-137">JSON representation</span></span>

<span data-ttu-id="cd852-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd852-138">Here is a JSON representation of the resource.</span></span>

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