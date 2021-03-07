---
title: тип ресурса printTaskTrigger
description: Определяет условия, при которых будет выполнен новый printTask на основе связанного печатиTaskDefinition.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: c0871f936b0935e6a599e79d6fb1a75f7e28f7ed
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518016"
---
# <a name="printtasktrigger-resource-type"></a><span data-ttu-id="e95e9-103">тип ресурса printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="e95e9-103">printTaskTrigger resource type</span></span>

<span data-ttu-id="e95e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e95e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="e95e9-105">Определяет условие, при котором будет запускаться новый [printTask](printtask.md) на основе связанного с ним [принтаTaskDefinition.](printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e95e9-105">Determines the condition under which a new [printTask](printtask.md) will be triggered based on the associated [printTaskDefinition](printtaskdefinition.md).</span></span>

<span data-ttu-id="e95e9-106">Дополнительные сведения о том, как использовать этот ресурс для добавления поддержки печати в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="e95e9-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="e95e9-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e95e9-107">Methods</span></span>
|<span data-ttu-id="e95e9-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e95e9-108">Method</span></span>|<span data-ttu-id="e95e9-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="e95e9-109">Return type</span></span>|<span data-ttu-id="e95e9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e95e9-110">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="e95e9-111">Список</span><span class="sxs-lookup"><span data-stu-id="e95e9-111">List</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="e95e9-112">[printTaskTrigger](printtasktrigger.md) collection</span><span class="sxs-lookup"><span data-stu-id="e95e9-112">[printTaskTrigger](printtasktrigger.md) collection</span></span> | <span data-ttu-id="e95e9-113">Получите список printTaskTriggers, связанных с определенным [принтером.](printer.md)</span><span class="sxs-lookup"><span data-stu-id="e95e9-113">Get a list of printTaskTriggers associated with a particular [printer](printer.md).</span></span> |
| <span data-ttu-id="e95e9-114">[получение](../api/printtasktrigger-get.md);</span><span class="sxs-lookup"><span data-stu-id="e95e9-114">[Get](../api/printtasktrigger-get.md)</span></span> | [<span data-ttu-id="e95e9-115">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="e95e9-115">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="e95e9-116">Получите печатьTaskTrigger, связанную с определенным [printTask.](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="e95e9-116">Get the printTaskTrigger associated with a particular [printTask](printtask.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="e95e9-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="e95e9-117">Properties</span></span>
|<span data-ttu-id="e95e9-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="e95e9-118">Property</span></span>|<span data-ttu-id="e95e9-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e95e9-119">Type</span></span>|<span data-ttu-id="e95e9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e95e9-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e95e9-121">id</span><span class="sxs-lookup"><span data-stu-id="e95e9-121">id</span></span>|<span data-ttu-id="e95e9-122">Строка</span><span class="sxs-lookup"><span data-stu-id="e95e9-122">String</span></span>|<span data-ttu-id="e95e9-123">Идентификатор printTaskTrigger.</span><span class="sxs-lookup"><span data-stu-id="e95e9-123">The printTaskTrigger's identifier.</span></span> <span data-ttu-id="e95e9-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e95e9-124">Read-only.</span></span>|
|<span data-ttu-id="e95e9-125">event</span><span class="sxs-lookup"><span data-stu-id="e95e9-125">event</span></span>|<span data-ttu-id="e95e9-126">printEvent</span><span class="sxs-lookup"><span data-stu-id="e95e9-126">printEvent</span></span>|<span data-ttu-id="e95e9-127">Событие Universal Print, которое приведет к запуску новой [печатиTask.](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="e95e9-127">The Universal Print event that will cause a new [printTask](printtask.md) to be triggered.</span></span> <span data-ttu-id="e95e9-128">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="e95e9-128">Valid values are described in the following table.</span></span>|

### <a name="printevent-values"></a><span data-ttu-id="e95e9-129">printEvent values</span><span class="sxs-lookup"><span data-stu-id="e95e9-129">printEvent values</span></span>

|<span data-ttu-id="e95e9-130">Элемент</span><span class="sxs-lookup"><span data-stu-id="e95e9-130">Member</span></span>|<span data-ttu-id="e95e9-131">Значение</span><span class="sxs-lookup"><span data-stu-id="e95e9-131">Value</span></span>|<span data-ttu-id="e95e9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e95e9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e95e9-133">jobStarted</span><span class="sxs-lookup"><span data-stu-id="e95e9-133">jobStarted</span></span>|<span data-ttu-id="e95e9-134">0</span><span class="sxs-lookup"><span data-stu-id="e95e9-134">0</span></span>|<span data-ttu-id="e95e9-135">Представляет событие, которое происходит при работе с новой печатью.</span><span class="sxs-lookup"><span data-stu-id="e95e9-135">Represents an event that occurs when a new print job is started.</span></span>|
|<span data-ttu-id="e95e9-136">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="e95e9-136">unknownFutureValue</span></span>|<span data-ttu-id="e95e9-137">1 </span><span class="sxs-lookup"><span data-stu-id="e95e9-137">1</span></span>|<span data-ttu-id="e95e9-138">Эволюционирующее значение sentinel.</span><span class="sxs-lookup"><span data-stu-id="e95e9-138">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="e95e9-139">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="e95e9-139">Do not use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e95e9-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="e95e9-140">Relationships</span></span>
|<span data-ttu-id="e95e9-141">Связь</span><span class="sxs-lookup"><span data-stu-id="e95e9-141">Relationship</span></span>|<span data-ttu-id="e95e9-142">Тип</span><span class="sxs-lookup"><span data-stu-id="e95e9-142">Type</span></span>|<span data-ttu-id="e95e9-143">Описание</span><span class="sxs-lookup"><span data-stu-id="e95e9-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e95e9-144">определение</span><span class="sxs-lookup"><span data-stu-id="e95e9-144">definition</span></span>|[<span data-ttu-id="e95e9-145">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="e95e9-145">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="e95e9-146">Абстрактное определение, которое будет использоваться для создания [printTask](printtask.md) при запуске события печати.</span><span class="sxs-lookup"><span data-stu-id="e95e9-146">An abstract definition that will be used to create a [printTask](printtask.md) when triggered by a print event.</span></span> <span data-ttu-id="e95e9-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e95e9-147">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e95e9-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e95e9-148">JSON representation</span></span>
<span data-ttu-id="e95e9-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e95e9-149">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printTaskTrigger",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskTrigger",
  "id": "String (identifier)",
  "event": "String"
}
```

