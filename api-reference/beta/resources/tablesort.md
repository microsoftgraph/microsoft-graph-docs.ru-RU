---
title: Тип ресурса TableSort
description: Управляет операциями сортировки для объектов Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5e5e93fb1cccb420e8da08015109c81dc45ae688
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966491"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="6959c-103">Тип ресурса TableSort</span><span class="sxs-lookup"><span data-stu-id="6959c-103">TableSort resource type</span></span>

> <span data-ttu-id="6959c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6959c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6959c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6959c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6959c-106">Управляет операциями сортировки для объектов Table.</span><span class="sxs-lookup"><span data-stu-id="6959c-106">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="6959c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6959c-107">Methods</span></span>

| <span data-ttu-id="6959c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="6959c-108">Method</span></span>           | <span data-ttu-id="6959c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6959c-109">Return Type</span></span>    |<span data-ttu-id="6959c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6959c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6959c-111">Получение объекта TableSort</span><span class="sxs-lookup"><span data-stu-id="6959c-111">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="6959c-112">TableSort</span><span class="sxs-lookup"><span data-stu-id="6959c-112">TableSort</span></span>](tablesort.md) |<span data-ttu-id="6959c-113">Чтение свойств и связей объекта tableSort.</span><span class="sxs-lookup"><span data-stu-id="6959c-113">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="6959c-114">Apply</span><span class="sxs-lookup"><span data-stu-id="6959c-114">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="6959c-115">Нет</span><span class="sxs-lookup"><span data-stu-id="6959c-115">None</span></span>|<span data-ttu-id="6959c-116">Выполняет сортировку.</span><span class="sxs-lookup"><span data-stu-id="6959c-116">Perform a sort operation.</span></span>|
|[<span data-ttu-id="6959c-117">Clear</span><span class="sxs-lookup"><span data-stu-id="6959c-117">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="6959c-118">Нет</span><span class="sxs-lookup"><span data-stu-id="6959c-118">None</span></span>|<span data-ttu-id="6959c-p102">Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="6959c-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="6959c-121">Reapply</span><span class="sxs-lookup"><span data-stu-id="6959c-121">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="6959c-122">Нет</span><span class="sxs-lookup"><span data-stu-id="6959c-122">None</span></span>|<span data-ttu-id="6959c-123">Повторно применяет текущие параметры сортировки к таблице.</span><span class="sxs-lookup"><span data-stu-id="6959c-123">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="6959c-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="6959c-124">Properties</span></span>
| <span data-ttu-id="6959c-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="6959c-125">Property</span></span>     | <span data-ttu-id="6959c-126">Тип</span><span class="sxs-lookup"><span data-stu-id="6959c-126">Type</span></span>   |<span data-ttu-id="6959c-127">Описание</span><span class="sxs-lookup"><span data-stu-id="6959c-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6959c-128">matchCase</span><span class="sxs-lookup"><span data-stu-id="6959c-128">matchCase</span></span>|<span data-ttu-id="6959c-129">boolean</span><span class="sxs-lookup"><span data-stu-id="6959c-129">boolean</span></span>|<span data-ttu-id="6959c-p103">Указывает, учитывался ли регистр при последней сортировке таблице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6959c-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="6959c-132">method</span><span class="sxs-lookup"><span data-stu-id="6959c-132">method</span></span>|<span data-ttu-id="6959c-133">строка</span><span class="sxs-lookup"><span data-stu-id="6959c-133">string</span></span>|<span data-ttu-id="6959c-p104">Указывает метод сортировки китайских символов, который использовался при последней сортировке таблицы. Возможные значения: `PinYin`, `StrokeCount`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6959c-p104">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6959c-137">Связи</span><span class="sxs-lookup"><span data-stu-id="6959c-137">Relationships</span></span>
| <span data-ttu-id="6959c-138">Связь</span><span class="sxs-lookup"><span data-stu-id="6959c-138">Relationship</span></span> | <span data-ttu-id="6959c-139">Тип</span><span class="sxs-lookup"><span data-stu-id="6959c-139">Type</span></span>   |<span data-ttu-id="6959c-140">Описание</span><span class="sxs-lookup"><span data-stu-id="6959c-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6959c-141">fields</span><span class="sxs-lookup"><span data-stu-id="6959c-141">fields</span></span>|[<span data-ttu-id="6959c-142">SortField</span><span class="sxs-lookup"><span data-stu-id="6959c-142">SortField</span></span>](sortfield.md)|<span data-ttu-id="6959c-p105">Указывает текущие условия, которые использовались при последней сортировке таблицы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6959c-p105">Represents the current conditions used to last sort the table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6959c-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6959c-145">JSON representation</span></span>

<span data-ttu-id="6959c-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6959c-146">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
