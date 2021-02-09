---
title: Тип ресурса assignmentFilterEvaluationSummary
description: Представляем сводку результатов для оценки фильтра назначений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 31f2e93f481f0b21689b1a83d63f4540c22f50cb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160900"
---
# <a name="assignmentfilterevaluationsummary-resource-type"></a><span data-ttu-id="1018b-103">Тип ресурса assignmentFilterEvaluationSummary</span><span class="sxs-lookup"><span data-stu-id="1018b-103">assignmentFilterEvaluationSummary resource type</span></span>

<span data-ttu-id="1018b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1018b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1018b-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1018b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1018b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1018b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1018b-107">Представляем сводку результатов для оценки фильтра назначений</span><span class="sxs-lookup"><span data-stu-id="1018b-107">Represent result summary for assignment filter evaluation</span></span>

## <a name="properties"></a><span data-ttu-id="1018b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1018b-108">Properties</span></span>
|<span data-ttu-id="1018b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1018b-109">Property</span></span>|<span data-ttu-id="1018b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1018b-110">Type</span></span>|<span data-ttu-id="1018b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1018b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1018b-112">assignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="1018b-112">assignmentFilterId</span></span>|<span data-ttu-id="1018b-113">String</span><span class="sxs-lookup"><span data-stu-id="1018b-113">String</span></span>|<span data-ttu-id="1018b-114">Уникальный идентификатор объекта фильтра назначений</span><span class="sxs-lookup"><span data-stu-id="1018b-114">Unique identifier for the assignment filter object</span></span>|
|<span data-ttu-id="1018b-115">assignmentFilterLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1018b-115">assignmentFilterLastModifiedDateTime</span></span>|<span data-ttu-id="1018b-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1018b-116">DateTimeOffset</span></span>|<span data-ttu-id="1018b-117">Время последнего изменения фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="1018b-117">The time the assignment filter was last modified.</span></span>|
|<span data-ttu-id="1018b-118">assignmentFilterDisplayName</span><span class="sxs-lookup"><span data-stu-id="1018b-118">assignmentFilterDisplayName</span></span>|<span data-ttu-id="1018b-119">String</span><span class="sxs-lookup"><span data-stu-id="1018b-119">String</span></span>|<span data-ttu-id="1018b-120">Имя фильтра назначений, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="1018b-120">The admin defined name for assignment filter.</span></span>|
|<span data-ttu-id="1018b-121">assignmentFilterPlatform</span><span class="sxs-lookup"><span data-stu-id="1018b-121">assignmentFilterPlatform</span></span>|[<span data-ttu-id="1018b-122">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="1018b-122">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="1018b-123">Платформа, для которой создается фильтр назначений.</span><span class="sxs-lookup"><span data-stu-id="1018b-123">The platform for which this assignment filter is created.</span></span> <span data-ttu-id="1018b-124">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="1018b-124">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="1018b-125">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="1018b-125">evaluationResult</span></span>|[<span data-ttu-id="1018b-126">assignmentFilterEvaluationResult</span><span class="sxs-lookup"><span data-stu-id="1018b-126">assignmentFilterEvaluationResult</span></span>](../resources/intune-policyset-assignmentfilterevaluationresult.md)|<span data-ttu-id="1018b-127">Результат оценки фильтра назначений.</span><span class="sxs-lookup"><span data-stu-id="1018b-127">Assignment filter evaluation result.</span></span> <span data-ttu-id="1018b-128">Возможные значения: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.</span><span class="sxs-lookup"><span data-stu-id="1018b-128">Possible values are: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.</span></span>|
|<span data-ttu-id="1018b-129">evaluationDateTime</span><span class="sxs-lookup"><span data-stu-id="1018b-129">evaluationDateTime</span></span>|<span data-ttu-id="1018b-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1018b-130">DateTimeOffset</span></span>|<span data-ttu-id="1018b-131">Был оценен фильтр назначения времени.</span><span class="sxs-lookup"><span data-stu-id="1018b-131">The time assignment filter was evaluated.</span></span>|
|<span data-ttu-id="1018b-132">assignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="1018b-132">assignmentFilterType</span></span>|[<span data-ttu-id="1018b-133">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="1018b-133">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="1018b-134">Указать тип фильтра, включаемого или исключаемого.</span><span class="sxs-lookup"><span data-stu-id="1018b-134">Indicate filter type either include or exclude.</span></span> <span data-ttu-id="1018b-135">Возможные значения: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="1018b-135">Possible values are: `none`, `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1018b-136">Связи</span><span class="sxs-lookup"><span data-stu-id="1018b-136">Relationships</span></span>
<span data-ttu-id="1018b-137">Нет</span><span class="sxs-lookup"><span data-stu-id="1018b-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1018b-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1018b-138">JSON Representation</span></span>
<span data-ttu-id="1018b-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1018b-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterEvaluationSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationSummary",
  "assignmentFilterId": "String",
  "assignmentFilterLastModifiedDateTime": "String (timestamp)",
  "assignmentFilterDisplayName": "String",
  "assignmentFilterPlatform": "String",
  "evaluationResult": "String",
  "evaluationDateTime": "String (timestamp)",
  "assignmentFilterType": "String"
}
```




