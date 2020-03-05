---
title: Тип ресурса Воркбукаппликатион
description: Представляет приложение Excel, которое управляет книгой.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d4b2833910d22696ee95ed707469f6da2068453c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446725"
---
# <a name="workbookapplication-resource-type"></a><span data-ttu-id="8426a-103">Тип ресурса Воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="8426a-103">workbookApplication resource type</span></span>

<span data-ttu-id="8426a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8426a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8426a-105">Представляет приложение Excel, которое управляет книгой.</span><span class="sxs-lookup"><span data-stu-id="8426a-105">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="8426a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8426a-106">Methods</span></span>

| <span data-ttu-id="8426a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8426a-107">Method</span></span>           | <span data-ttu-id="8426a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8426a-108">Return Type</span></span>    |<span data-ttu-id="8426a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8426a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8426a-110">Получение Воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="8426a-110">Get workbookApplication</span></span>](../api/workbookapplication-get.md) | [<span data-ttu-id="8426a-111">воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="8426a-111">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="8426a-112">Чтение свойств и связей объекта Воркбукаппликатион.</span><span class="sxs-lookup"><span data-stu-id="8426a-112">Read properties and relationships of workbookApplication object.</span></span>|
|[<span data-ttu-id="8426a-113">Calculate</span><span class="sxs-lookup"><span data-stu-id="8426a-113">Calculate</span></span>](../api/workbookapplication-calculate.md)|<span data-ttu-id="8426a-114">Нет</span><span class="sxs-lookup"><span data-stu-id="8426a-114">None</span></span>|<span data-ttu-id="8426a-115">Пересчитывает данные во всех открытых в текущий момент книгах Excel.</span><span class="sxs-lookup"><span data-stu-id="8426a-115">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="8426a-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="8426a-116">Properties</span></span>
| <span data-ttu-id="8426a-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="8426a-117">Property</span></span>     | <span data-ttu-id="8426a-118">Тип</span><span class="sxs-lookup"><span data-stu-id="8426a-118">Type</span></span>   |<span data-ttu-id="8426a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8426a-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8426a-120">калкулатионмоде</span><span class="sxs-lookup"><span data-stu-id="8426a-120">calculationMode</span></span>|<span data-ttu-id="8426a-121">string</span><span class="sxs-lookup"><span data-stu-id="8426a-121">string</span></span>|<span data-ttu-id="8426a-122">Возвращает режим вычисления, который используется в книге.</span><span class="sxs-lookup"><span data-stu-id="8426a-122">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="8426a-123">Возможные значения: `Automatic`, `AutomaticExceptTables`, `Manual`.</span><span class="sxs-lookup"><span data-stu-id="8426a-123">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8426a-124">Связи</span><span class="sxs-lookup"><span data-stu-id="8426a-124">Relationships</span></span>
<span data-ttu-id="8426a-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8426a-125">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="8426a-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8426a-126">JSON representation</span></span>

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
