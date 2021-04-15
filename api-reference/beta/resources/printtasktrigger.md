---
title: тип ресурса printTaskTrigger
description: Определяет условия, при которых будет выполнен новый printTask на основе связанного печатиTaskDefinition.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: de2da4f94894d9744fdfdd302b310251cd91fdb3
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766324"
---
# <a name="printtasktrigger-resource-type"></a><span data-ttu-id="eb4ad-103">тип ресурса printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="eb4ad-103">printTaskTrigger resource type</span></span>

<span data-ttu-id="eb4ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb4ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb4ad-105">Определяет условие, при котором будет запускаться новый [printTask](printtask.md) на основе связанного с ним [принтаTaskDefinition.](printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="eb4ad-105">Determines the condition under which a new [printTask](printtask.md) will be triggered based on the associated [printTaskDefinition](printtaskdefinition.md).</span></span>

<span data-ttu-id="eb4ad-106">Дополнительные сведения о том, как использовать этот ресурс для добавления поддержки печати в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="eb4ad-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="eb4ad-107">Методы</span><span class="sxs-lookup"><span data-stu-id="eb4ad-107">Methods</span></span>

| <span data-ttu-id="eb4ad-108">Метод</span><span class="sxs-lookup"><span data-stu-id="eb4ad-108">Method</span></span>       | <span data-ttu-id="eb4ad-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eb4ad-109">Return Type</span></span> | <span data-ttu-id="eb4ad-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eb4ad-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="eb4ad-111">Список</span><span class="sxs-lookup"><span data-stu-id="eb4ad-111">List</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="eb4ad-112">[printTaskTrigger](printtasktrigger.md) collection</span><span class="sxs-lookup"><span data-stu-id="eb4ad-112">[printTaskTrigger](printtasktrigger.md) collection</span></span> | <span data-ttu-id="eb4ad-113">Получите список printTaskTriggers, связанных с определенным [принтером.](printer.md)</span><span class="sxs-lookup"><span data-stu-id="eb4ad-113">Get a list of printTaskTriggers associated with a particular [printer](printer.md).</span></span> |
| [<span data-ttu-id="eb4ad-114">Get</span><span class="sxs-lookup"><span data-stu-id="eb4ad-114">Get</span></span>](../api/printtasktrigger-get.md) | [<span data-ttu-id="eb4ad-115">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="eb4ad-115">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="eb4ad-116">Получите определенный шрифтTaskTrigger, связанный с определенным [принтером.](printer.md)</span><span class="sxs-lookup"><span data-stu-id="eb4ad-116">Get a particular printTaskTrigger associated with a particular [printer](printer.md).</span></span>|


## <a name="properties"></a><span data-ttu-id="eb4ad-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb4ad-117">Properties</span></span>
| <span data-ttu-id="eb4ad-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb4ad-118">Property</span></span>     | <span data-ttu-id="eb4ad-119">Тип</span><span class="sxs-lookup"><span data-stu-id="eb4ad-119">Type</span></span>        | <span data-ttu-id="eb4ad-120">Описание</span><span class="sxs-lookup"><span data-stu-id="eb4ad-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eb4ad-121">id</span><span class="sxs-lookup"><span data-stu-id="eb4ad-121">id</span></span>|<span data-ttu-id="eb4ad-122">String</span><span class="sxs-lookup"><span data-stu-id="eb4ad-122">String</span></span>|<span data-ttu-id="eb4ad-123">Идентификатор printTaskTrigger.</span><span class="sxs-lookup"><span data-stu-id="eb4ad-123">The printTaskTrigger's identifier.</span></span> <span data-ttu-id="eb4ad-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eb4ad-124">Read-only.</span></span>|
|<span data-ttu-id="eb4ad-125">event</span><span class="sxs-lookup"><span data-stu-id="eb4ad-125">event</span></span>|<span data-ttu-id="eb4ad-126">printEvent</span><span class="sxs-lookup"><span data-stu-id="eb4ad-126">printEvent</span></span>|<span data-ttu-id="eb4ad-127">Событие Universal Print, которое приведет к запуску новой [печатиTask.](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="eb4ad-127">The Universal Print event that will cause a new [printTask](printtask.md) to be triggered.</span></span> <span data-ttu-id="eb4ad-128">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="eb4ad-128">Valid values are described in the following table.</span></span>|

### <a name="printevent-values"></a><span data-ttu-id="eb4ad-129">printEvent values</span><span class="sxs-lookup"><span data-stu-id="eb4ad-129">printEvent values</span></span>

|<span data-ttu-id="eb4ad-130">Элемент</span><span class="sxs-lookup"><span data-stu-id="eb4ad-130">Member</span></span>|<span data-ttu-id="eb4ad-131">Значение</span><span class="sxs-lookup"><span data-stu-id="eb4ad-131">Value</span></span>|<span data-ttu-id="eb4ad-132">Описание</span><span class="sxs-lookup"><span data-stu-id="eb4ad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb4ad-133">jobStarted</span><span class="sxs-lookup"><span data-stu-id="eb4ad-133">jobStarted</span></span>|<span data-ttu-id="eb4ad-134">0</span><span class="sxs-lookup"><span data-stu-id="eb4ad-134">0</span></span>|<span data-ttu-id="eb4ad-135">Представляет событие, которое происходит при работе с новой печатью.</span><span class="sxs-lookup"><span data-stu-id="eb4ad-135">Represents an event that occurs when a new print job is started.</span></span>|
|<span data-ttu-id="eb4ad-136">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="eb4ad-136">unknownFutureValue</span></span>|<span data-ttu-id="eb4ad-137">1</span><span class="sxs-lookup"><span data-stu-id="eb4ad-137">1</span></span>|<span data-ttu-id="eb4ad-138">Эволюционирующее значение sentinel.</span><span class="sxs-lookup"><span data-stu-id="eb4ad-138">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="eb4ad-139">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="eb4ad-139">Do not use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb4ad-140">Связи</span><span class="sxs-lookup"><span data-stu-id="eb4ad-140">Relationships</span></span>
| <span data-ttu-id="eb4ad-141">Связь</span><span class="sxs-lookup"><span data-stu-id="eb4ad-141">Relationship</span></span> | <span data-ttu-id="eb4ad-142">Тип</span><span class="sxs-lookup"><span data-stu-id="eb4ad-142">Type</span></span>        | <span data-ttu-id="eb4ad-143">Описание</span><span class="sxs-lookup"><span data-stu-id="eb4ad-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eb4ad-144">определение</span><span class="sxs-lookup"><span data-stu-id="eb4ad-144">definition</span></span>|[<span data-ttu-id="eb4ad-145">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="eb4ad-145">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="eb4ad-146">Абстрактное определение, которое будет использоваться для создания [printTask](printtask.md) при запуске события печати.</span><span class="sxs-lookup"><span data-stu-id="eb4ad-146">An abstract definition that will be used to create a [printTask](printtask.md) when triggered by a print event.</span></span> <span data-ttu-id="eb4ad-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eb4ad-147">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb4ad-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb4ad-148">JSON representation</span></span>

<span data-ttu-id="eb4ad-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb4ad-149">The following is a JSON representation of the resource.</span></span>

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


