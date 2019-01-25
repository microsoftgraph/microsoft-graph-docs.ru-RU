---
title: Тип ресурса TableSort
description: Управляет операциями сортировки для объектов Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 612e0cb7d59011f04ae992f80119fc1da572b582
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511746"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="6d4f0-103">Тип ресурса TableSort</span><span class="sxs-lookup"><span data-stu-id="6d4f0-103">TableSort resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d4f0-104">Управляет операциями сортировки для объектов Table.</span><span class="sxs-lookup"><span data-stu-id="6d4f0-104">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="6d4f0-105">Методы</span><span class="sxs-lookup"><span data-stu-id="6d4f0-105">Methods</span></span>

| <span data-ttu-id="6d4f0-106">Метод</span><span class="sxs-lookup"><span data-stu-id="6d4f0-106">Method</span></span>           | <span data-ttu-id="6d4f0-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6d4f0-107">Return Type</span></span>    |<span data-ttu-id="6d4f0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6d4f0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d4f0-109">Получение объекта TableSort</span><span class="sxs-lookup"><span data-stu-id="6d4f0-109">[Get TableSort](../api/tablesort-get.md)</span></span> | [<span data-ttu-id="6d4f0-110">TableSort</span><span class="sxs-lookup"><span data-stu-id="6d4f0-110">TableSort</span></span>](tablesort.md) |<span data-ttu-id="6d4f0-111">Чтение свойств и связей объекта tableSort.</span><span class="sxs-lookup"><span data-stu-id="6d4f0-111">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="6d4f0-112">Apply</span><span class="sxs-lookup"><span data-stu-id="6d4f0-112">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="6d4f0-113">Нет</span><span class="sxs-lookup"><span data-stu-id="6d4f0-113">None</span></span>|<span data-ttu-id="6d4f0-114">Выполняет сортировку.</span><span class="sxs-lookup"><span data-stu-id="6d4f0-114">Perform a sort operation.</span></span>|
|[<span data-ttu-id="6d4f0-115">Clear</span><span class="sxs-lookup"><span data-stu-id="6d4f0-115">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="6d4f0-116">Нет</span><span class="sxs-lookup"><span data-stu-id="6d4f0-116">None</span></span>|<span data-ttu-id="6d4f0-p101">Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="6d4f0-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="6d4f0-119">Reapply</span><span class="sxs-lookup"><span data-stu-id="6d4f0-119">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="6d4f0-120">Нет</span><span class="sxs-lookup"><span data-stu-id="6d4f0-120">None</span></span>|<span data-ttu-id="6d4f0-121">Повторно применяет текущие параметры сортировки к таблице.</span><span class="sxs-lookup"><span data-stu-id="6d4f0-121">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="6d4f0-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d4f0-122">Properties</span></span>
| <span data-ttu-id="6d4f0-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d4f0-123">Property</span></span>     | <span data-ttu-id="6d4f0-124">Тип</span><span class="sxs-lookup"><span data-stu-id="6d4f0-124">Type</span></span>   |<span data-ttu-id="6d4f0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="6d4f0-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d4f0-126">matchCase</span><span class="sxs-lookup"><span data-stu-id="6d4f0-126">matchCase</span></span>|<span data-ttu-id="6d4f0-127">boolean</span><span class="sxs-lookup"><span data-stu-id="6d4f0-127">boolean</span></span>|<span data-ttu-id="6d4f0-p102">Указывает, учитывался ли регистр при последней сортировке таблице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6d4f0-p102">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="6d4f0-130">method</span><span class="sxs-lookup"><span data-stu-id="6d4f0-130">method</span></span>|<span data-ttu-id="6d4f0-131">string</span><span class="sxs-lookup"><span data-stu-id="6d4f0-131">string</span></span>|<span data-ttu-id="6d4f0-p103">Указывает метод сортировки китайских символов, который использовался при последней сортировке таблицы. Возможные значения: `PinYin`, `StrokeCount`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6d4f0-p103">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d4f0-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="6d4f0-135">Relationships</span></span>
| <span data-ttu-id="6d4f0-136">Связь</span><span class="sxs-lookup"><span data-stu-id="6d4f0-136">Relationship</span></span> | <span data-ttu-id="6d4f0-137">Тип</span><span class="sxs-lookup"><span data-stu-id="6d4f0-137">Type</span></span>   |<span data-ttu-id="6d4f0-138">Описание</span><span class="sxs-lookup"><span data-stu-id="6d4f0-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d4f0-139">fields</span><span class="sxs-lookup"><span data-stu-id="6d4f0-139">fields</span></span>|[<span data-ttu-id="6d4f0-140">SortField</span><span class="sxs-lookup"><span data-stu-id="6d4f0-140">SortField</span></span>](sortfield.md)|<span data-ttu-id="6d4f0-p104">Указывает текущие условия, которые использовались при последней сортировке таблицы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6d4f0-p104">Represents the current conditions used to last sort the table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d4f0-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d4f0-143">JSON representation</span></span>

<span data-ttu-id="6d4f0-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d4f0-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/tablesort.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
