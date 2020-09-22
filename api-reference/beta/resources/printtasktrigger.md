---
title: Тип ресурса Принттасктригжер
description: Определяет условия, при которых новый Принттаск будет выполняться на основе связанного Принттаскдефинитион.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: fc05fe9011d91ac9da5f74a6079537ebfba25160
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078294"
---
# <a name="printtasktrigger-resource-type"></a><span data-ttu-id="bc1ee-103">Тип ресурса Принттасктригжер</span><span class="sxs-lookup"><span data-stu-id="bc1ee-103">printTaskTrigger resource type</span></span>

<span data-ttu-id="bc1ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc1ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc1ee-105">Определяет условие, при котором новый [принттаск](printtask.md) будет запускаться на основе связанного [принттаскдефинитион](printtaskdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="bc1ee-105">Determines the condition under which a new [printTask](printtask.md) will be triggered based on the associated [printTaskDefinition](printtaskdefinition.md).</span></span>

<span data-ttu-id="bc1ee-106">Дополнительные сведения о том, как использовать этот ресурс для поддержки печати по запросу в универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="bc1ee-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="bc1ee-107">Методы</span><span class="sxs-lookup"><span data-stu-id="bc1ee-107">Methods</span></span>

| <span data-ttu-id="bc1ee-108">Метод</span><span class="sxs-lookup"><span data-stu-id="bc1ee-108">Method</span></span>       | <span data-ttu-id="bc1ee-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bc1ee-109">Return Type</span></span> | <span data-ttu-id="bc1ee-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bc1ee-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bc1ee-111">Список</span><span class="sxs-lookup"><span data-stu-id="bc1ee-111">List</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="bc1ee-112">Коллекция [принттасктригжер](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="bc1ee-112">[printTaskTrigger](printtasktrigger.md) collection</span></span> | <span data-ttu-id="bc1ee-113">Получение списка Принттасктригжерс, связанных с определенным [принтером](printer.md).</span><span class="sxs-lookup"><span data-stu-id="bc1ee-113">Get a list of printTaskTriggers associated with a particular [printer](printer.md).</span></span> |
| <span data-ttu-id="bc1ee-114">[получение](../api/printtasktrigger-get.md);</span><span class="sxs-lookup"><span data-stu-id="bc1ee-114">[Get](../api/printtasktrigger-get.md)</span></span> | [<span data-ttu-id="bc1ee-115">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="bc1ee-115">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="bc1ee-116">Получение Принттасктригжер, связанного с определенным [принттаск](printtask.md).</span><span class="sxs-lookup"><span data-stu-id="bc1ee-116">Get the printTaskTrigger associated with a particular [printTask](printtask.md).</span></span> |


## <a name="properties"></a><span data-ttu-id="bc1ee-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc1ee-117">Properties</span></span>
| <span data-ttu-id="bc1ee-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc1ee-118">Property</span></span>     | <span data-ttu-id="bc1ee-119">Тип</span><span class="sxs-lookup"><span data-stu-id="bc1ee-119">Type</span></span>        | <span data-ttu-id="bc1ee-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bc1ee-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bc1ee-121">id</span><span class="sxs-lookup"><span data-stu-id="bc1ee-121">id</span></span>|<span data-ttu-id="bc1ee-122">String</span><span class="sxs-lookup"><span data-stu-id="bc1ee-122">String</span></span>|<span data-ttu-id="bc1ee-123">Идентификатор Принттасктригжер.</span><span class="sxs-lookup"><span data-stu-id="bc1ee-123">The printTaskTrigger's identifier.</span></span> <span data-ttu-id="bc1ee-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc1ee-124">Read-only.</span></span>|
|<span data-ttu-id="bc1ee-125">event</span><span class="sxs-lookup"><span data-stu-id="bc1ee-125">event</span></span>|<span data-ttu-id="bc1ee-126">принтевент</span><span class="sxs-lookup"><span data-stu-id="bc1ee-126">printEvent</span></span>|<span data-ttu-id="bc1ee-127">Универсальное событие печати, которое вызывает срабатывание нового [принттаск](printtask.md) .</span><span class="sxs-lookup"><span data-stu-id="bc1ee-127">The Universal Print event that will cause a new [printTask](printtask.md) to be triggered.</span></span> <span data-ttu-id="bc1ee-128">Допустимые значения описаны в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="bc1ee-128">Valid values are described in the following table.</span></span>|

### <a name="printevent-values"></a><span data-ttu-id="bc1ee-129">значения Принтевент</span><span class="sxs-lookup"><span data-stu-id="bc1ee-129">printEvent values</span></span>

|<span data-ttu-id="bc1ee-130">Элемент</span><span class="sxs-lookup"><span data-stu-id="bc1ee-130">Member</span></span>|<span data-ttu-id="bc1ee-131">Значение</span><span class="sxs-lookup"><span data-stu-id="bc1ee-131">Value</span></span>|<span data-ttu-id="bc1ee-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bc1ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc1ee-133">жобстартед</span><span class="sxs-lookup"><span data-stu-id="bc1ee-133">jobStarted</span></span>|<span data-ttu-id="bc1ee-134">нуль</span><span class="sxs-lookup"><span data-stu-id="bc1ee-134">0</span></span>|<span data-ttu-id="bc1ee-135">Представляет событие, возникающее при запуске нового задания печати.</span><span class="sxs-lookup"><span data-stu-id="bc1ee-135">Represents an event that occurs when a new print job is started.</span></span>|
|<span data-ttu-id="bc1ee-136">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="bc1ee-136">unknownFutureValue</span></span>|<span data-ttu-id="bc1ee-137">1 </span><span class="sxs-lookup"><span data-stu-id="bc1ee-137">1</span></span>|<span data-ttu-id="bc1ee-138">Значение Sentinel для перечисления расширяемые.</span><span class="sxs-lookup"><span data-stu-id="bc1ee-138">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="bc1ee-139">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="bc1ee-139">Do not use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc1ee-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="bc1ee-140">Relationships</span></span>
| <span data-ttu-id="bc1ee-141">Связь</span><span class="sxs-lookup"><span data-stu-id="bc1ee-141">Relationship</span></span> | <span data-ttu-id="bc1ee-142">Тип</span><span class="sxs-lookup"><span data-stu-id="bc1ee-142">Type</span></span>        | <span data-ttu-id="bc1ee-143">Описание</span><span class="sxs-lookup"><span data-stu-id="bc1ee-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bc1ee-144">RDLC</span><span class="sxs-lookup"><span data-stu-id="bc1ee-144">definition</span></span>|[<span data-ttu-id="bc1ee-145">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="bc1ee-145">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="bc1ee-146">Абстрактное определение, которое будет использоваться для создания объекта [принттаск](printtask.md) при запуске события Print.</span><span class="sxs-lookup"><span data-stu-id="bc1ee-146">An abstract definition that will be used to create a [printTask](printtask.md) when triggered by a print event.</span></span> <span data-ttu-id="bc1ee-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc1ee-147">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc1ee-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc1ee-148">JSON representation</span></span>

<span data-ttu-id="bc1ee-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc1ee-149">The following is a JSON representation of the resource.</span></span>

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


