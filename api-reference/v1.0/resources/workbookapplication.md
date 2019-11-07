---
title: Тип ресурса Воркбукаппликатион
description: Представляет приложение Excel, которое управляет книгой.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a4f7d2cd6887598ac0a60522dc5bee1101dff9c9
ms.sourcegitcommit: 2f3e7325b5bc1f0cdc12a8acdf34d31cea3b8bdb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/07/2019
ms.locfileid: "38023250"
---
# <a name="workbookapplication-resource-type"></a><span data-ttu-id="1704a-103">Тип ресурса Воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="1704a-103">workbookApplication resource type</span></span>

<span data-ttu-id="1704a-104">Представляет приложение Excel, которое управляет книгой.</span><span class="sxs-lookup"><span data-stu-id="1704a-104">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="1704a-105">Методы</span><span class="sxs-lookup"><span data-stu-id="1704a-105">Methods</span></span>

| <span data-ttu-id="1704a-106">Метод</span><span class="sxs-lookup"><span data-stu-id="1704a-106">Method</span></span>           | <span data-ttu-id="1704a-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1704a-107">Return Type</span></span>    |<span data-ttu-id="1704a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1704a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1704a-109">Получение Воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="1704a-109">Get workbookApplication</span></span>](../api/workbookapplication-get.md) | [<span data-ttu-id="1704a-110">воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="1704a-110">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="1704a-111">Чтение свойств и связей объекта Воркбукаппликатион.</span><span class="sxs-lookup"><span data-stu-id="1704a-111">Read properties and relationships of workbookApplication object.</span></span>|
|[<span data-ttu-id="1704a-112">Calculate</span><span class="sxs-lookup"><span data-stu-id="1704a-112">Calculate</span></span>](../api/workbookapplication-calculate.md)|<span data-ttu-id="1704a-113">Нет</span><span class="sxs-lookup"><span data-stu-id="1704a-113">None</span></span>|<span data-ttu-id="1704a-114">Пересчитывает данные во всех открытых в текущий момент книгах Excel.</span><span class="sxs-lookup"><span data-stu-id="1704a-114">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="1704a-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="1704a-115">Properties</span></span>
| <span data-ttu-id="1704a-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="1704a-116">Property</span></span>     | <span data-ttu-id="1704a-117">Тип</span><span class="sxs-lookup"><span data-stu-id="1704a-117">Type</span></span>   |<span data-ttu-id="1704a-118">Описание</span><span class="sxs-lookup"><span data-stu-id="1704a-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1704a-119">калкулатионмоде</span><span class="sxs-lookup"><span data-stu-id="1704a-119">calculationMode</span></span>|<span data-ttu-id="1704a-120">string</span><span class="sxs-lookup"><span data-stu-id="1704a-120">string</span></span>|<span data-ttu-id="1704a-121">Возвращает режим вычисления, который используется в книге.</span><span class="sxs-lookup"><span data-stu-id="1704a-121">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="1704a-122">Возможные значения: `Automatic`, `AutomaticExceptTables`, `Manual`.</span><span class="sxs-lookup"><span data-stu-id="1704a-122">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1704a-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="1704a-123">Relationships</span></span>
<span data-ttu-id="1704a-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1704a-124">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="1704a-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1704a-125">JSON representation</span></span>

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
