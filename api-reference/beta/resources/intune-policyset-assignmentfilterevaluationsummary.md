---
title: тип ресурса assignmentFilterEvaluationSummary
description: Представляем сводку результатов для оценки фильтра назначения
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 05c9a3eabd22e7e22a6d74229b7aa47901e05db6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155983"
---
# <a name="assignmentfilterevaluationsummary-resource-type"></a><span data-ttu-id="55ff9-103">тип ресурса assignmentFilterEvaluationSummary</span><span class="sxs-lookup"><span data-stu-id="55ff9-103">assignmentFilterEvaluationSummary resource type</span></span>

<span data-ttu-id="55ff9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55ff9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55ff9-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55ff9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55ff9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55ff9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55ff9-107">Представляем сводку результатов для оценки фильтра назначения</span><span class="sxs-lookup"><span data-stu-id="55ff9-107">Represent result summary for assignment filter evaluation</span></span>

## <a name="properties"></a><span data-ttu-id="55ff9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="55ff9-108">Properties</span></span>
|<span data-ttu-id="55ff9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="55ff9-109">Property</span></span>|<span data-ttu-id="55ff9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="55ff9-110">Type</span></span>|<span data-ttu-id="55ff9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="55ff9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55ff9-112">assignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="55ff9-112">assignmentFilterId</span></span>|<span data-ttu-id="55ff9-113">Строка</span><span class="sxs-lookup"><span data-stu-id="55ff9-113">String</span></span>|<span data-ttu-id="55ff9-114">Уникальный идентификатор для объекта фильтра назначения</span><span class="sxs-lookup"><span data-stu-id="55ff9-114">Unique identifier for the assignment filter object</span></span>|
|<span data-ttu-id="55ff9-115">assignmentFilterLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55ff9-115">assignmentFilterLastModifiedDateTime</span></span>|<span data-ttu-id="55ff9-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55ff9-116">DateTimeOffset</span></span>|<span data-ttu-id="55ff9-117">Время последнего изменения фильтра назначения.</span><span class="sxs-lookup"><span data-stu-id="55ff9-117">The time the assignment filter was last modified.</span></span>|
|<span data-ttu-id="55ff9-118">assignmentFilterDisplayName</span><span class="sxs-lookup"><span data-stu-id="55ff9-118">assignmentFilterDisplayName</span></span>|<span data-ttu-id="55ff9-119">Строка</span><span class="sxs-lookup"><span data-stu-id="55ff9-119">String</span></span>|<span data-ttu-id="55ff9-120">Имя администратора для фильтра назначения.</span><span class="sxs-lookup"><span data-stu-id="55ff9-120">The admin defined name for assignment filter.</span></span>|
|<span data-ttu-id="55ff9-121">assignmentFilterPlatform</span><span class="sxs-lookup"><span data-stu-id="55ff9-121">assignmentFilterPlatform</span></span>|[<span data-ttu-id="55ff9-122">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="55ff9-122">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="55ff9-123">Платформа, для которой создается фильтр назначения.</span><span class="sxs-lookup"><span data-stu-id="55ff9-123">The platform for which this assignment filter is created.</span></span> <span data-ttu-id="55ff9-124">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="55ff9-124">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="55ff9-125">assessmentResult</span><span class="sxs-lookup"><span data-stu-id="55ff9-125">evaluationResult</span></span>|[<span data-ttu-id="55ff9-126">assignmentFilterEvaluationResult</span><span class="sxs-lookup"><span data-stu-id="55ff9-126">assignmentFilterEvaluationResult</span></span>](../resources/intune-policyset-assignmentfilterevaluationresult.md)|<span data-ttu-id="55ff9-127">Результат оценки фильтра назначения.</span><span class="sxs-lookup"><span data-stu-id="55ff9-127">Assignment filter evaluation result.</span></span> <span data-ttu-id="55ff9-128">Возможные значения: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.</span><span class="sxs-lookup"><span data-stu-id="55ff9-128">Possible values are: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.</span></span>|
|<span data-ttu-id="55ff9-129">assessmentDateTime</span><span class="sxs-lookup"><span data-stu-id="55ff9-129">evaluationDateTime</span></span>|<span data-ttu-id="55ff9-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55ff9-130">DateTimeOffset</span></span>|<span data-ttu-id="55ff9-131">Был оценен фильтр назначения времени.</span><span class="sxs-lookup"><span data-stu-id="55ff9-131">The time assignment filter was evaluated.</span></span>|
|<span data-ttu-id="55ff9-132">assignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="55ff9-132">assignmentFilterType</span></span>|[<span data-ttu-id="55ff9-133">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="55ff9-133">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="55ff9-134">Указать тип фильтра либо включить, либо исключить.</span><span class="sxs-lookup"><span data-stu-id="55ff9-134">Indicate filter type either include or exclude.</span></span> <span data-ttu-id="55ff9-135">Возможные значения: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="55ff9-135">Possible values are: `none`, `include`, `exclude`.</span></span>|
|<span data-ttu-id="55ff9-136">assignmentFilterTypeAndEvaluationResults</span><span class="sxs-lookup"><span data-stu-id="55ff9-136">assignmentFilterTypeAndEvaluationResults</span></span>|<span data-ttu-id="55ff9-137">[assignmentFilterTypeAndEvaluationResult](../resources/intune-policyset-assignmentfiltertypeandevaluationresult.md) collection</span><span class="sxs-lookup"><span data-stu-id="55ff9-137">[assignmentFilterTypeAndEvaluationResult](../resources/intune-policyset-assignmentfiltertypeandevaluationresult.md) collection</span></span>|<span data-ttu-id="55ff9-138">Коллекция типов фильтров и их соответствующих результатов оценки.</span><span class="sxs-lookup"><span data-stu-id="55ff9-138">A collection of filter types and their corresponding evaluation results.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55ff9-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="55ff9-139">Relationships</span></span>
<span data-ttu-id="55ff9-140">Нет</span><span class="sxs-lookup"><span data-stu-id="55ff9-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55ff9-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55ff9-141">JSON Representation</span></span>
<span data-ttu-id="55ff9-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55ff9-142">Here is a JSON representation of the resource.</span></span>
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
  "assignmentFilterType": "String",
  "assignmentFilterTypeAndEvaluationResults": [
    {
      "@odata.type": "microsoft.graph.assignmentFilterTypeAndEvaluationResult",
      "assignmentFilterType": "String",
      "evaluationResult": "String"
    }
  ]
}
```




