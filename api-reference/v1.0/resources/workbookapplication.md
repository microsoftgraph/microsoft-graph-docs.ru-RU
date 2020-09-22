---
title: Тип ресурса Воркбукаппликатион
description: Представляет приложение Excel, которое управляет книгой.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 36626698d55fe8dc813d13d66a7fa453f8e2beae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015164"
---
# <a name="workbookapplication-resource-type"></a><span data-ttu-id="0c1ba-103">Тип ресурса Воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="0c1ba-103">workbookApplication resource type</span></span>

<span data-ttu-id="0c1ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c1ba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0c1ba-105">Представляет приложение Excel, которое управляет книгой.</span><span class="sxs-lookup"><span data-stu-id="0c1ba-105">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="0c1ba-106">Методы</span><span class="sxs-lookup"><span data-stu-id="0c1ba-106">Methods</span></span>

| <span data-ttu-id="0c1ba-107">Метод</span><span class="sxs-lookup"><span data-stu-id="0c1ba-107">Method</span></span>           | <span data-ttu-id="0c1ba-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0c1ba-108">Return Type</span></span>    |<span data-ttu-id="0c1ba-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0c1ba-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0c1ba-110">Получение Воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="0c1ba-110">Get workbookApplication</span></span>](../api/workbookapplication-get.md) | [<span data-ttu-id="0c1ba-111">воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="0c1ba-111">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="0c1ba-112">Чтение свойств и связей объекта Воркбукаппликатион.</span><span class="sxs-lookup"><span data-stu-id="0c1ba-112">Read properties and relationships of workbookApplication object.</span></span>|
|[<span data-ttu-id="0c1ba-113">Calculate</span><span class="sxs-lookup"><span data-stu-id="0c1ba-113">Calculate</span></span>](../api/workbookapplication-calculate.md)|<span data-ttu-id="0c1ba-114">Нет</span><span class="sxs-lookup"><span data-stu-id="0c1ba-114">None</span></span>|<span data-ttu-id="0c1ba-115">Пересчитывает данные во всех открытых в текущий момент книгах Excel.</span><span class="sxs-lookup"><span data-stu-id="0c1ba-115">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="0c1ba-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c1ba-116">Properties</span></span>
| <span data-ttu-id="0c1ba-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c1ba-117">Property</span></span>     | <span data-ttu-id="0c1ba-118">Тип</span><span class="sxs-lookup"><span data-stu-id="0c1ba-118">Type</span></span>   |<span data-ttu-id="0c1ba-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0c1ba-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c1ba-120">калкулатионмоде</span><span class="sxs-lookup"><span data-stu-id="0c1ba-120">calculationMode</span></span>|<span data-ttu-id="0c1ba-121">string</span><span class="sxs-lookup"><span data-stu-id="0c1ba-121">string</span></span>|<span data-ttu-id="0c1ba-122">Возвращает режим вычисления, который используется в книге.</span><span class="sxs-lookup"><span data-stu-id="0c1ba-122">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="0c1ba-123">Возможные значения: `Automatic`, `AutomaticExceptTables`, `Manual`.</span><span class="sxs-lookup"><span data-stu-id="0c1ba-123">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c1ba-124">Связи</span><span class="sxs-lookup"><span data-stu-id="0c1ba-124">Relationships</span></span>
<span data-ttu-id="0c1ba-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0c1ba-125">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0c1ba-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c1ba-126">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookApplication"
}-->

```json
{
  "calculationMode": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

