---
title: Тип ресурса Воркбукаппликатион
description: Представляет Воркбукаппликатион Excel, который управляет книгой.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 71c7c92e623fc2a9c05b9e1e8448f329615c51e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964111"
---
# <a name="workbookapplication-resource-type"></a><span data-ttu-id="9fdd4-103">Тип ресурса Воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="9fdd4-103">workbookApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fdd4-104">Представляет приложение Excel, которое управляет книгой.</span><span class="sxs-lookup"><span data-stu-id="9fdd4-104">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="9fdd4-105">Методы</span><span class="sxs-lookup"><span data-stu-id="9fdd4-105">Methods</span></span>

| <span data-ttu-id="9fdd4-106">Метод</span><span class="sxs-lookup"><span data-stu-id="9fdd4-106">Method</span></span>           | <span data-ttu-id="9fdd4-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9fdd4-107">Return Type</span></span>    |<span data-ttu-id="9fdd4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9fdd4-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9fdd4-109">Получение Воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="9fdd4-109">Get workbookApplication</span></span>](../api/workbookapplication-get.md) | [<span data-ttu-id="9fdd4-110">Воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="9fdd4-110">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="9fdd4-111">Чтение свойств и связей объекта Воркбукаппликатион.</span><span class="sxs-lookup"><span data-stu-id="9fdd4-111">Read properties and relationships of workbookApplication object.</span></span>|
|[<span data-ttu-id="9fdd4-112">Calculate</span><span class="sxs-lookup"><span data-stu-id="9fdd4-112">Calculate</span></span>](../api/workbookapplication-calculate.md)|<span data-ttu-id="9fdd4-113">Нет</span><span class="sxs-lookup"><span data-stu-id="9fdd4-113">None</span></span>|<span data-ttu-id="9fdd4-114">Пересчитывает данные во всех открытых в текущий момент книгах Excel.</span><span class="sxs-lookup"><span data-stu-id="9fdd4-114">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="9fdd4-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fdd4-115">Properties</span></span>
| <span data-ttu-id="9fdd4-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fdd4-116">Property</span></span>     | <span data-ttu-id="9fdd4-117">Тип</span><span class="sxs-lookup"><span data-stu-id="9fdd4-117">Type</span></span>   |<span data-ttu-id="9fdd4-118">Описание</span><span class="sxs-lookup"><span data-stu-id="9fdd4-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fdd4-119">Калкулатионмоде</span><span class="sxs-lookup"><span data-stu-id="9fdd4-119">calculationMode</span></span>|<span data-ttu-id="9fdd4-120">string</span><span class="sxs-lookup"><span data-stu-id="9fdd4-120">string</span></span>|<span data-ttu-id="9fdd4-121">Возвращает режим вычисления, который используется в книге.</span><span class="sxs-lookup"><span data-stu-id="9fdd4-121">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="9fdd4-122">Возможные значения: `Automatic`, `AutomaticExceptTables`, `Manual`.</span><span class="sxs-lookup"><span data-stu-id="9fdd4-122">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span> <span data-ttu-id="9fdd4-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9fdd4-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fdd4-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="9fdd4-124">Relationships</span></span>
<span data-ttu-id="9fdd4-125">Нет</span><span class="sxs-lookup"><span data-stu-id="9fdd4-125">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9fdd4-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fdd4-126">JSON representation</span></span>

<span data-ttu-id="9fdd4-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fdd4-127">Here is a JSON representation of the resource.</span></span>

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
