---
title: Тип ресурса TableSort
description: Управляет операциями сортировки для объектов Table.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 7e3eae5ef21bc8d8ea1fba395b369ea35d1f80b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873047"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="98a3e-103">Тип ресурса TableSort</span><span class="sxs-lookup"><span data-stu-id="98a3e-103">TableSort resource type</span></span>

> <span data-ttu-id="98a3e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="98a3e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98a3e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98a3e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="98a3e-106">Управляет операциями сортировки для объектов Table.</span><span class="sxs-lookup"><span data-stu-id="98a3e-106">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="98a3e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="98a3e-107">Methods</span></span>

| <span data-ttu-id="98a3e-108">Метод</span><span class="sxs-lookup"><span data-stu-id="98a3e-108">Method</span></span>           | <span data-ttu-id="98a3e-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="98a3e-109">Return Type</span></span>    |<span data-ttu-id="98a3e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="98a3e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="98a3e-111">Получение объекта TableSort</span><span class="sxs-lookup"><span data-stu-id="98a3e-111">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="98a3e-112">TableSort</span><span class="sxs-lookup"><span data-stu-id="98a3e-112">TableSort</span></span>](tablesort.md) |<span data-ttu-id="98a3e-113">Чтение свойств и связей объекта tableSort.</span><span class="sxs-lookup"><span data-stu-id="98a3e-113">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="98a3e-114">Apply</span><span class="sxs-lookup"><span data-stu-id="98a3e-114">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="98a3e-115">Нет</span><span class="sxs-lookup"><span data-stu-id="98a3e-115">None</span></span>|<span data-ttu-id="98a3e-116">Выполняет сортировку.</span><span class="sxs-lookup"><span data-stu-id="98a3e-116">Perform a sort operation.</span></span>|
|[<span data-ttu-id="98a3e-117">Clear</span><span class="sxs-lookup"><span data-stu-id="98a3e-117">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="98a3e-118">Нет</span><span class="sxs-lookup"><span data-stu-id="98a3e-118">None</span></span>|<span data-ttu-id="98a3e-p102">Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="98a3e-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="98a3e-121">Reapply</span><span class="sxs-lookup"><span data-stu-id="98a3e-121">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="98a3e-122">Нет</span><span class="sxs-lookup"><span data-stu-id="98a3e-122">None</span></span>|<span data-ttu-id="98a3e-123">Повторно применяет текущие параметры сортировки к таблице.</span><span class="sxs-lookup"><span data-stu-id="98a3e-123">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="98a3e-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="98a3e-124">Properties</span></span>
| <span data-ttu-id="98a3e-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="98a3e-125">Property</span></span>     | <span data-ttu-id="98a3e-126">Тип</span><span class="sxs-lookup"><span data-stu-id="98a3e-126">Type</span></span>   |<span data-ttu-id="98a3e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="98a3e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98a3e-128">matchCase</span><span class="sxs-lookup"><span data-stu-id="98a3e-128">matchCase</span></span>|<span data-ttu-id="98a3e-129">boolean</span><span class="sxs-lookup"><span data-stu-id="98a3e-129">boolean</span></span>|<span data-ttu-id="98a3e-p103">Указывает, учитывался ли регистр при последней сортировке таблице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98a3e-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="98a3e-132">method</span><span class="sxs-lookup"><span data-stu-id="98a3e-132">method</span></span>|<span data-ttu-id="98a3e-133">string</span><span class="sxs-lookup"><span data-stu-id="98a3e-133">string</span></span>|<span data-ttu-id="98a3e-p104">Указывает метод сортировки китайских символов, который использовался при последней сортировке таблицы. Возможные значения: `PinYin`, `StrokeCount`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98a3e-p104">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98a3e-137">Связи</span><span class="sxs-lookup"><span data-stu-id="98a3e-137">Relationships</span></span>
| <span data-ttu-id="98a3e-138">Связь</span><span class="sxs-lookup"><span data-stu-id="98a3e-138">Relationship</span></span> | <span data-ttu-id="98a3e-139">Тип</span><span class="sxs-lookup"><span data-stu-id="98a3e-139">Type</span></span>   |<span data-ttu-id="98a3e-140">Описание</span><span class="sxs-lookup"><span data-stu-id="98a3e-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98a3e-141">fields</span><span class="sxs-lookup"><span data-stu-id="98a3e-141">fields</span></span>|[<span data-ttu-id="98a3e-142">SortField</span><span class="sxs-lookup"><span data-stu-id="98a3e-142">SortField</span></span>](sortfield.md)|<span data-ttu-id="98a3e-p105">Указывает текущие условия, которые использовались при последней сортировке таблицы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98a3e-p105">Represents the current conditions used to last sort the table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98a3e-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98a3e-145">JSON representation</span></span>

<span data-ttu-id="98a3e-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98a3e-146">Here is a JSON representation of the resource.</span></span>

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
