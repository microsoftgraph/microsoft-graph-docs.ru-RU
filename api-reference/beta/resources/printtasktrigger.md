---
title: Тип ресурса Принттасктригжер
description: Определяет условия, при которых новый Принттаск будет выполняться на основе связанного Принттаскдефинитион.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 0a9ca4d06f43c9dd0964f0bb4c9614bfb4a78c1e
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091696"
---
# <a name="printtasktrigger-resource-type"></a><span data-ttu-id="69eb1-103">Тип ресурса Принттасктригжер</span><span class="sxs-lookup"><span data-stu-id="69eb1-103">printTaskTrigger resource type</span></span>

<span data-ttu-id="69eb1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69eb1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69eb1-105">Определяет условие, при котором новый [принттаск](printtask.md) будет запускаться на основе связанного [принттаскдефинитион](printtaskdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="69eb1-105">Determines the condition under which a new [printTask](printtask.md) will be triggered based on the associated [printTaskDefinition](printtaskdefinition.md).</span></span>

<span data-ttu-id="69eb1-106">Дополнительные сведения о том, как использовать этот ресурс для поддержки печати по запросу в универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="69eb1-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="69eb1-107">Методы</span><span class="sxs-lookup"><span data-stu-id="69eb1-107">Methods</span></span>

| <span data-ttu-id="69eb1-108">Метод</span><span class="sxs-lookup"><span data-stu-id="69eb1-108">Method</span></span>       | <span data-ttu-id="69eb1-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="69eb1-109">Return Type</span></span> | <span data-ttu-id="69eb1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="69eb1-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="69eb1-111">Список</span><span class="sxs-lookup"><span data-stu-id="69eb1-111">List</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="69eb1-112">Коллекция [принттасктригжер](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="69eb1-112">[printTaskTrigger](printtasktrigger.md) collection</span></span> | <span data-ttu-id="69eb1-113">Получение списка Принттасктригжерс, связанных с определенным [принтером](printer.md).</span><span class="sxs-lookup"><span data-stu-id="69eb1-113">Get a list of printTaskTriggers associated with a particular [printer](printer.md).</span></span> |
| [<span data-ttu-id="69eb1-114">Get</span><span class="sxs-lookup"><span data-stu-id="69eb1-114">Get</span></span>](../api/printtasktrigger-get.md) | [<span data-ttu-id="69eb1-115">принттасктригжер</span><span class="sxs-lookup"><span data-stu-id="69eb1-115">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="69eb1-116">Получение Принттасктригжер, связанного с определенным [принттаск](printtask.md).</span><span class="sxs-lookup"><span data-stu-id="69eb1-116">Get the printTaskTrigger associated with a particular [printTask](printtask.md).</span></span> |


## <a name="properties"></a><span data-ttu-id="69eb1-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="69eb1-117">Properties</span></span>
| <span data-ttu-id="69eb1-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="69eb1-118">Property</span></span>     | <span data-ttu-id="69eb1-119">Тип</span><span class="sxs-lookup"><span data-stu-id="69eb1-119">Type</span></span>        | <span data-ttu-id="69eb1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="69eb1-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="69eb1-121">id</span><span class="sxs-lookup"><span data-stu-id="69eb1-121">id</span></span>|<span data-ttu-id="69eb1-122">String</span><span class="sxs-lookup"><span data-stu-id="69eb1-122">String</span></span>|<span data-ttu-id="69eb1-123">Идентификатор Принттасктригжер.</span><span class="sxs-lookup"><span data-stu-id="69eb1-123">The printTaskTrigger's identifier.</span></span> <span data-ttu-id="69eb1-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69eb1-124">Read-only.</span></span>|
|<span data-ttu-id="69eb1-125">event</span><span class="sxs-lookup"><span data-stu-id="69eb1-125">event</span></span>|<span data-ttu-id="69eb1-126">принтевент</span><span class="sxs-lookup"><span data-stu-id="69eb1-126">printEvent</span></span>|<span data-ttu-id="69eb1-127">Универсальное событие печати, которое вызывает срабатывание нового [принттаск](printtask.md) .</span><span class="sxs-lookup"><span data-stu-id="69eb1-127">The Universal Print event that will cause a new [printTask](printtask.md) to be triggered.</span></span> <span data-ttu-id="69eb1-128">Допустимые значения описаны в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="69eb1-128">Valid values are described in the following table.</span></span>|

### <a name="printevent-values"></a><span data-ttu-id="69eb1-129">значения Принтевент</span><span class="sxs-lookup"><span data-stu-id="69eb1-129">printEvent values</span></span>

|<span data-ttu-id="69eb1-130">Элемент</span><span class="sxs-lookup"><span data-stu-id="69eb1-130">Member</span></span>|<span data-ttu-id="69eb1-131">Значение</span><span class="sxs-lookup"><span data-stu-id="69eb1-131">Value</span></span>|<span data-ttu-id="69eb1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="69eb1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69eb1-133">жобстартед</span><span class="sxs-lookup"><span data-stu-id="69eb1-133">jobStarted</span></span>|<span data-ttu-id="69eb1-134">нуль</span><span class="sxs-lookup"><span data-stu-id="69eb1-134">0</span></span>|<span data-ttu-id="69eb1-135">Представляет событие, возникающее при запуске нового задания печати.</span><span class="sxs-lookup"><span data-stu-id="69eb1-135">Represents an event that occurs when a new print job is started.</span></span>|
|<span data-ttu-id="69eb1-136">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="69eb1-136">unknownFutureValue</span></span>|<span data-ttu-id="69eb1-137">1 </span><span class="sxs-lookup"><span data-stu-id="69eb1-137">1</span></span>|<span data-ttu-id="69eb1-138">Значение Sentinel для перечисления расширяемые.</span><span class="sxs-lookup"><span data-stu-id="69eb1-138">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="69eb1-139">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="69eb1-139">Do not use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69eb1-140">Связи</span><span class="sxs-lookup"><span data-stu-id="69eb1-140">Relationships</span></span>
| <span data-ttu-id="69eb1-141">Связь</span><span class="sxs-lookup"><span data-stu-id="69eb1-141">Relationship</span></span> | <span data-ttu-id="69eb1-142">Тип</span><span class="sxs-lookup"><span data-stu-id="69eb1-142">Type</span></span>        | <span data-ttu-id="69eb1-143">Описание</span><span class="sxs-lookup"><span data-stu-id="69eb1-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="69eb1-144">RDLC</span><span class="sxs-lookup"><span data-stu-id="69eb1-144">definition</span></span>|[<span data-ttu-id="69eb1-145">принттаскдефинитион</span><span class="sxs-lookup"><span data-stu-id="69eb1-145">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="69eb1-146">Абстрактное определение, которое будет использоваться для создания объекта [принттаск](printtask.md) при запуске события Print.</span><span class="sxs-lookup"><span data-stu-id="69eb1-146">An abstract definition that will be used to create a [printTask](printtask.md) when triggered by a print event.</span></span> <span data-ttu-id="69eb1-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69eb1-147">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69eb1-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69eb1-148">JSON representation</span></span>

<span data-ttu-id="69eb1-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69eb1-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskTrigger",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "event": {"@odata.type": "microsoft.graph.printEvent"},
  "definition": {"@odata.type": "microsoft.graph.printTaskDefinition"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
