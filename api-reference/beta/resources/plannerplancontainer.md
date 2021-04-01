---
title: тип ресурса plannerPlanContainer
description: Представляет контейнер для планировщикаPlan. Контейнер — это ресурс, который указывает правила авторизации и срок службы плана.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: acb7a85683bc94795953e524ee9630d6cfc01f24
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473887"
---
# <a name="plannerplancontainer-resource-type"></a><span data-ttu-id="955b8-104">тип ресурса plannerPlanContainer</span><span class="sxs-lookup"><span data-stu-id="955b8-104">plannerPlanContainer resource type</span></span>

<span data-ttu-id="955b8-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="955b8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="955b8-106">Представляет контейнер для [планировщикаPlan](plannerPlan.md).</span><span class="sxs-lookup"><span data-stu-id="955b8-106">Represents a container for a [plannerPlan](plannerPlan.md).</span></span> <span data-ttu-id="955b8-107">Контейнер — это ресурс, который указывает правила авторизации и срок службы плана.</span><span class="sxs-lookup"><span data-stu-id="955b8-107">The container is a resource that specifies authorization rules and the lifetime of the plan.</span></span> <span data-ttu-id="955b8-108">Это означает, что только те, кто уполномочен работать с ресурсом, содержащим план, смогут работать с планом и задачами в нем.</span><span class="sxs-lookup"><span data-stu-id="955b8-108">This means that only the people who are authorized to work with the resource containing the plan will be able to work with the plan and the tasks within it.</span></span> <span data-ttu-id="955b8-109">При удалении содержащего ресурса также удаляются содержащиеся планы.</span><span class="sxs-lookup"><span data-stu-id="955b8-109">When the containing resource is deleted, the contained plans are also deleted.</span></span> <span data-ttu-id="955b8-110">Свойства **планировщикаPlanContainer** не могут быть изменены после создания плана.</span><span class="sxs-lookup"><span data-stu-id="955b8-110">Properties of **plannerPlanContainer** cannot be changed after the plan is created.</span></span>

<span data-ttu-id="955b8-111">Планировщик в настоящее время поддерживает типы контейнеров, перечисленные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="955b8-111">Planner currently supports the container types listed in the following table.</span></span> <span data-ttu-id="955b8-112">При создании плана свойство **containerUrl** должно быть указано с помощью пути ресурса, указанного в таблице.</span><span class="sxs-lookup"><span data-stu-id="955b8-112">When creating a plan, the **containerUrl** property must be specified with the path of the resource identified in the table.</span></span>

|<span data-ttu-id="955b8-113">Тип</span><span class="sxs-lookup"><span data-stu-id="955b8-113">Type</span></span>|<span data-ttu-id="955b8-114">Описание</span><span class="sxs-lookup"><span data-stu-id="955b8-114">Description</span></span>|<span data-ttu-id="955b8-115">Путь к ресурсу</span><span class="sxs-lookup"><span data-stu-id="955b8-115">Path to the resource</span></span>|
|----|-----------|--------------------|
|<span data-ttu-id="955b8-116">group</span><span class="sxs-lookup"><span data-stu-id="955b8-116">group</span></span>| <span data-ttu-id="955b8-117">План содержится [группой](group.md).</span><span class="sxs-lookup"><span data-stu-id="955b8-117">Plan is contained by a [group](group.md).</span></span>| <span data-ttu-id="955b8-118"> https://graph.microsoft.com/beta/groups/&lt;id&gt;</span><span class="sxs-lookup"><span data-stu-id="955b8-118">https://graph.microsoft.com/beta/groups/&lt;id&gt;</span></span>|
|<span data-ttu-id="955b8-119">реестр</span><span class="sxs-lookup"><span data-stu-id="955b8-119">roster</span></span>| <span data-ttu-id="955b8-120">План содержится [планировщикомRoster](plannerroster.md)</span><span class="sxs-lookup"><span data-stu-id="955b8-120">Plan is contained by a [plannerRoster](plannerroster.md)</span></span> | <span data-ttu-id="955b8-121"> https://graph.microsoft.com/beta/planner/rosters/&lt;id&gt;</span><span class="sxs-lookup"><span data-stu-id="955b8-121">https://graph.microsoft.com/beta/planner/rosters/&lt;id&gt;</span></span>|

## <a name="properties"></a><span data-ttu-id="955b8-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="955b8-122">Properties</span></span>
|<span data-ttu-id="955b8-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="955b8-123">Property</span></span>|<span data-ttu-id="955b8-124">Тип</span><span class="sxs-lookup"><span data-stu-id="955b8-124">Type</span></span>|<span data-ttu-id="955b8-125">Описание</span><span class="sxs-lookup"><span data-stu-id="955b8-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="955b8-126">containerId</span><span class="sxs-lookup"><span data-stu-id="955b8-126">containerId</span></span>|<span data-ttu-id="955b8-127">String</span><span class="sxs-lookup"><span data-stu-id="955b8-127">String</span></span>|<span data-ttu-id="955b8-128">Идентификатор ресурса, который содержит план.</span><span class="sxs-lookup"><span data-stu-id="955b8-128">The identifier of the resource that contains the plan.</span></span>|
|<span data-ttu-id="955b8-129">type</span><span class="sxs-lookup"><span data-stu-id="955b8-129">type</span></span>|<span data-ttu-id="955b8-130">plannerContainerType</span><span class="sxs-lookup"><span data-stu-id="955b8-130">plannerContainerType</span></span>| <span data-ttu-id="955b8-131">Тип ресурса, который содержит план.</span><span class="sxs-lookup"><span data-stu-id="955b8-131">The type of the resource that contains the plan.</span></span> <span data-ttu-id="955b8-132">См. предыдущую таблицу поддерживаемых типов.</span><span class="sxs-lookup"><span data-stu-id="955b8-132">See the previous table for supported types.</span></span> <span data-ttu-id="955b8-133">Возможные значения: `group`, `roster`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="955b8-133">Possible values are: `group`, `roster`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="955b8-134">url</span><span class="sxs-lookup"><span data-stu-id="955b8-134">url</span></span>|<span data-ttu-id="955b8-135">String</span><span class="sxs-lookup"><span data-stu-id="955b8-135">String</span></span>|<span data-ttu-id="955b8-136">Полный канонический URL-адрес контейнера.</span><span class="sxs-lookup"><span data-stu-id="955b8-136">The full canonical URL of the container.</span></span>|

## <a name="relationships"></a><span data-ttu-id="955b8-137">Связи</span><span class="sxs-lookup"><span data-stu-id="955b8-137">Relationships</span></span>
<span data-ttu-id="955b8-138">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="955b8-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="955b8-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="955b8-139">JSON representation</span></span>
<span data-ttu-id="955b8-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="955b8-140">The following is a JSON representation of the resource.</span></span>
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

