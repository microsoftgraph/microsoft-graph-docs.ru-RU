---
title: Тип ресурса Воркбукаппликатион
description: Представляет Воркбукаппликатион Excel, который управляет книгой.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 4616b3e61fbea3b918ef897ebe69dd12ffb0dbb2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039183"
---
# <a name="workbookapplication-resource-type"></a><span data-ttu-id="c6221-103">Тип ресурса Воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="c6221-103">workbookApplication resource type</span></span>

<span data-ttu-id="c6221-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6221-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6221-105">Представляет приложение Excel, которое управляет книгой.</span><span class="sxs-lookup"><span data-stu-id="c6221-105">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="c6221-106">Методы</span><span class="sxs-lookup"><span data-stu-id="c6221-106">Methods</span></span>

| <span data-ttu-id="c6221-107">Метод</span><span class="sxs-lookup"><span data-stu-id="c6221-107">Method</span></span>           | <span data-ttu-id="c6221-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c6221-108">Return Type</span></span>    |<span data-ttu-id="c6221-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c6221-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c6221-110">Получение Воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="c6221-110">Get workbookApplication</span></span>](../api/workbookapplication-get.md) | [<span data-ttu-id="c6221-111">воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="c6221-111">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="c6221-112">Чтение свойств и связей объекта Воркбукаппликатион.</span><span class="sxs-lookup"><span data-stu-id="c6221-112">Read properties and relationships of workbookApplication object.</span></span>|
|[<span data-ttu-id="c6221-113">Calculate</span><span class="sxs-lookup"><span data-stu-id="c6221-113">Calculate</span></span>](../api/workbookapplication-calculate.md)|<span data-ttu-id="c6221-114">Нет</span><span class="sxs-lookup"><span data-stu-id="c6221-114">None</span></span>|<span data-ttu-id="c6221-115">Пересчитывает данные во всех открытых в текущий момент книгах Excel.</span><span class="sxs-lookup"><span data-stu-id="c6221-115">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="c6221-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6221-116">Properties</span></span>
| <span data-ttu-id="c6221-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6221-117">Property</span></span>     | <span data-ttu-id="c6221-118">Тип</span><span class="sxs-lookup"><span data-stu-id="c6221-118">Type</span></span>   |<span data-ttu-id="c6221-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c6221-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6221-120">калкулатионмоде</span><span class="sxs-lookup"><span data-stu-id="c6221-120">calculationMode</span></span>|<span data-ttu-id="c6221-121">string</span><span class="sxs-lookup"><span data-stu-id="c6221-121">string</span></span>|<span data-ttu-id="c6221-122">Возвращает режим вычисления, который используется в книге.</span><span class="sxs-lookup"><span data-stu-id="c6221-122">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="c6221-123">Возможные значения: `Automatic`, `AutomaticExceptTables`, `Manual`.</span><span class="sxs-lookup"><span data-stu-id="c6221-123">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6221-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="c6221-124">Relationships</span></span>
<span data-ttu-id="c6221-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c6221-125">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="c6221-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c6221-126">JSON representation</span></span>


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


