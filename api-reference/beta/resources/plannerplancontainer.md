---
title: Тип ресурса plannerPlanContainer
description: Представляет контейнер для plannerPlan. Контейнер — это ресурс, который определяет правила авторизации и срок действия плана.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8b3abb10892077159e6f02c33a31d501a75dba2a
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883255"
---
# <a name="plannerplancontainer-resource-type"></a><span data-ttu-id="8c614-104">Тип ресурса plannerPlanContainer</span><span class="sxs-lookup"><span data-stu-id="8c614-104">plannerPlanContainer resource type</span></span>

<span data-ttu-id="8c614-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c614-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8c614-106">Представляет контейнер для [plannerPlan.](plannerPlan.md)</span><span class="sxs-lookup"><span data-stu-id="8c614-106">Represents a container for a [plannerPlan](plannerPlan.md).</span></span> <span data-ttu-id="8c614-107">Контейнер — это ресурс, который определяет правила авторизации и срок действия плана.</span><span class="sxs-lookup"><span data-stu-id="8c614-107">The container is a resource that specifies authorization rules and the lifetime of the plan.</span></span> <span data-ttu-id="8c614-108">Это означает, что только люди, которым разрешено работать с ресурсом, содержащим план, смогут работать с планом и задачами в нем.</span><span class="sxs-lookup"><span data-stu-id="8c614-108">This means that only the people who are authorized to work with the resource containing the plan will be able to work with the plan and the tasks within it.</span></span> <span data-ttu-id="8c614-109">При удалении содержащегося ресурса также удаляются содержащиеся планы.</span><span class="sxs-lookup"><span data-stu-id="8c614-109">When the containing resource is deleted, the contained plans are also deleted.</span></span> <span data-ttu-id="8c614-110">Свойства **объекта plannerPlanContainer** нельзя изменить после создания плана.</span><span class="sxs-lookup"><span data-stu-id="8c614-110">Properties of **plannerPlanContainer** cannot be changed after the plan is created.</span></span>

<span data-ttu-id="8c614-111">Планировщик в настоящее время поддерживает типы контейнеров, перечисленные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="8c614-111">Planner currently supports the container types listed in the following table.</span></span> <span data-ttu-id="8c614-112">При создании плана свойство **containerUrl** должно быть указано с помощью пути к ресурсу, указанному в таблице.</span><span class="sxs-lookup"><span data-stu-id="8c614-112">When creating a plan, the **containerUrl** property must be specified with the path of the resource identified in the table.</span></span>

|<span data-ttu-id="8c614-113">Тип</span><span class="sxs-lookup"><span data-stu-id="8c614-113">Type</span></span>|<span data-ttu-id="8c614-114">Описание</span><span class="sxs-lookup"><span data-stu-id="8c614-114">Description</span></span>|<span data-ttu-id="8c614-115">Путь к ресурсу</span><span class="sxs-lookup"><span data-stu-id="8c614-115">Path to the resource</span></span>|
|----|-----------|--------------------|
|<span data-ttu-id="8c614-116">group</span><span class="sxs-lookup"><span data-stu-id="8c614-116">group</span></span>| <span data-ttu-id="8c614-117">План содержится в группе.</span><span class="sxs-lookup"><span data-stu-id="8c614-117">Plan is contained by a group.</span></span>| <span data-ttu-id="8c614-118"> https://graph.microsoft.com/v1.0/groups/&lt;id&gt;</span><span class="sxs-lookup"><span data-stu-id="8c614-118">https://graph.microsoft.com/v1.0/groups/&lt;id&gt;</span></span>|

## <a name="properties"></a><span data-ttu-id="8c614-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c614-119">Properties</span></span>
|<span data-ttu-id="8c614-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c614-120">Property</span></span>|<span data-ttu-id="8c614-121">Тип</span><span class="sxs-lookup"><span data-stu-id="8c614-121">Type</span></span>|<span data-ttu-id="8c614-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8c614-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c614-123">containerId</span><span class="sxs-lookup"><span data-stu-id="8c614-123">containerId</span></span>|<span data-ttu-id="8c614-124">Строка</span><span class="sxs-lookup"><span data-stu-id="8c614-124">String</span></span>|<span data-ttu-id="8c614-125">Идентификатор ресурса, который содержит план.</span><span class="sxs-lookup"><span data-stu-id="8c614-125">The identifier of the resource that contains the plan.</span></span>|
|<span data-ttu-id="8c614-126">type</span><span class="sxs-lookup"><span data-stu-id="8c614-126">type</span></span>|<span data-ttu-id="8c614-127">plannerContainerType</span><span class="sxs-lookup"><span data-stu-id="8c614-127">plannerContainerType</span></span>| <span data-ttu-id="8c614-128">Тип ресурса, который содержит план.</span><span class="sxs-lookup"><span data-stu-id="8c614-128">The type of the resource that contains the plan.</span></span> <span data-ttu-id="8c614-129">Поддерживаемые типы см. в предыдущей таблице.</span><span class="sxs-lookup"><span data-stu-id="8c614-129">See the previous table for supported types.</span></span> <span data-ttu-id="8c614-130">Возможные значения: `group`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8c614-130">Possible values are: `group`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8c614-131">url</span><span class="sxs-lookup"><span data-stu-id="8c614-131">url</span></span>|<span data-ttu-id="8c614-132">String</span><span class="sxs-lookup"><span data-stu-id="8c614-132">String</span></span>|<span data-ttu-id="8c614-133">Полный канонический URL-адрес контейнера.</span><span class="sxs-lookup"><span data-stu-id="8c614-133">The full canonical URL of the container.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c614-134">Связи</span><span class="sxs-lookup"><span data-stu-id="8c614-134">Relationships</span></span>
<span data-ttu-id="8c614-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8c614-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c614-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8c614-136">JSON representation</span></span>
<span data-ttu-id="8c614-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c614-137">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerPlanContainer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerPlanContainer",
  "url": "String",
  "containerId": "String",
  "type": "String"
}
```

