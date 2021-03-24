---
title: тип ресурса assignmentFilterTypeAndEvaluationResult
description: Представляет тип фильтра и результат evalaution фильтра.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f969660fed52d3bdc3c37643d4502ff722cbee0d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146794"
---
# <a name="assignmentfiltertypeandevaluationresult-resource-type"></a><span data-ttu-id="c8112-103">тип ресурса assignmentFilterTypeAndEvaluationResult</span><span class="sxs-lookup"><span data-stu-id="c8112-103">assignmentFilterTypeAndEvaluationResult resource type</span></span>

<span data-ttu-id="c8112-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8112-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8112-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8112-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8112-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8112-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8112-107">Представляет тип фильтра и результат evalaution фильтра.</span><span class="sxs-lookup"><span data-stu-id="c8112-107">Represents the filter type and evalaution result of the filter.</span></span>

## <a name="properties"></a><span data-ttu-id="c8112-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8112-108">Properties</span></span>
|<span data-ttu-id="c8112-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8112-109">Property</span></span>|<span data-ttu-id="c8112-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c8112-110">Type</span></span>|<span data-ttu-id="c8112-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c8112-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8112-112">assignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="c8112-112">assignmentFilterType</span></span>|[<span data-ttu-id="c8112-113">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="c8112-113">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="c8112-114">Представляет тип фильтра.</span><span class="sxs-lookup"><span data-stu-id="c8112-114">Represents the filter type.</span></span> <span data-ttu-id="c8112-115">Возможные значения: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="c8112-115">Possible values are: `none`, `include`, `exclude`.</span></span>|
|<span data-ttu-id="c8112-116">assessmentResult</span><span class="sxs-lookup"><span data-stu-id="c8112-116">evaluationResult</span></span>|[<span data-ttu-id="c8112-117">assignmentFilterEvaluationResult</span><span class="sxs-lookup"><span data-stu-id="c8112-117">assignmentFilterEvaluationResult</span></span>](../resources/intune-policyset-assignmentfilterevaluationresult.md)|<span data-ttu-id="c8112-118">Представляет результат evalaution фильтра.</span><span class="sxs-lookup"><span data-stu-id="c8112-118">Represents the evalaution result of the filter.</span></span> <span data-ttu-id="c8112-119">Возможные значения: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.</span><span class="sxs-lookup"><span data-stu-id="c8112-119">Possible values are: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8112-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="c8112-120">Relationships</span></span>
<span data-ttu-id="c8112-121">Нет</span><span class="sxs-lookup"><span data-stu-id="c8112-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8112-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c8112-122">JSON Representation</span></span>
<span data-ttu-id="c8112-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8112-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterTypeAndEvaluationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterTypeAndEvaluationResult",
  "assignmentFilterType": "String",
  "evaluationResult": "String"
}
```




