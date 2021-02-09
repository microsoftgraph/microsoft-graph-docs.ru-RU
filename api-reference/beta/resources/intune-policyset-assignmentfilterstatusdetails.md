---
title: Тип ресурса assignmentFilterStatusDetails
description: Представляет сведения о состоянии для устройства и полезной нагрузки, а также всех связанных примененных фильтров.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a376b1ff3d554753120860f1d3541f7952dd6130
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160897"
---
# <a name="assignmentfilterstatusdetails-resource-type"></a><span data-ttu-id="6930f-103">Тип ресурса assignmentFilterStatusDetails</span><span class="sxs-lookup"><span data-stu-id="6930f-103">assignmentFilterStatusDetails resource type</span></span>

<span data-ttu-id="6930f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6930f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6930f-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6930f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6930f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6930f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6930f-107">Представляет сведения о состоянии для устройства и полезной нагрузки, а также всех связанных примененных фильтров.</span><span class="sxs-lookup"><span data-stu-id="6930f-107">Represent status details for device and payload and all associated applied filters.</span></span>

## <a name="properties"></a><span data-ttu-id="6930f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6930f-108">Properties</span></span>
|<span data-ttu-id="6930f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6930f-109">Property</span></span>|<span data-ttu-id="6930f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6930f-110">Type</span></span>|<span data-ttu-id="6930f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6930f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6930f-112">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="6930f-112">managedDeviceId</span></span>|<span data-ttu-id="6930f-113">String</span><span class="sxs-lookup"><span data-stu-id="6930f-113">String</span></span>|<span data-ttu-id="6930f-114">Уникальный идентификатор объекта устройства.</span><span class="sxs-lookup"><span data-stu-id="6930f-114">Unique identifier for the device object.</span></span>|
|<span data-ttu-id="6930f-115">payloadId</span><span class="sxs-lookup"><span data-stu-id="6930f-115">payloadId</span></span>|<span data-ttu-id="6930f-116">String</span><span class="sxs-lookup"><span data-stu-id="6930f-116">String</span></span>|<span data-ttu-id="6930f-117">Уникальный идентификатор объекта полезной нагрузки.</span><span class="sxs-lookup"><span data-stu-id="6930f-117">Unique identifier for payload object.</span></span>|
|<span data-ttu-id="6930f-118">userId</span><span class="sxs-lookup"><span data-stu-id="6930f-118">userId</span></span>|<span data-ttu-id="6930f-119">String</span><span class="sxs-lookup"><span data-stu-id="6930f-119">String</span></span>|<span data-ttu-id="6930f-120">Уникальный идентификатор объекта UserId.</span><span class="sxs-lookup"><span data-stu-id="6930f-120">Unique identifier for UserId object.</span></span> <span data-ttu-id="6930f-121">Может иметь null</span><span class="sxs-lookup"><span data-stu-id="6930f-121">Can be null</span></span>|
|<span data-ttu-id="6930f-122">deviceProperties</span><span class="sxs-lookup"><span data-stu-id="6930f-122">deviceProperties</span></span>|<span data-ttu-id="6930f-123">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6930f-123">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6930f-124">Свойства устройства, используемые для оценки фильтра во время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="6930f-124">Device properties used for filter evaluation during device check-in time.</span></span>|
|<span data-ttu-id="6930f-125">evalutionSummaries</span><span class="sxs-lookup"><span data-stu-id="6930f-125">evalutionSummaries</span></span>|<span data-ttu-id="6930f-126">[Коллекция assignmentFilterEvaluationSummary](../resources/intune-policyset-assignmentfilterevaluationsummary.md)</span><span class="sxs-lookup"><span data-stu-id="6930f-126">[assignmentFilterEvaluationSummary](../resources/intune-policyset-assignmentfilterevaluationsummary.md) collection</span></span>|<span data-ttu-id="6930f-127">Сводка результатов оценки для каждого фильтра, связанного с устройством и полезной нагрузкой</span><span class="sxs-lookup"><span data-stu-id="6930f-127">Evaluation result summaries for each filter associated to device and payload</span></span>|

## <a name="relationships"></a><span data-ttu-id="6930f-128">Связи</span><span class="sxs-lookup"><span data-stu-id="6930f-128">Relationships</span></span>
<span data-ttu-id="6930f-129">Нет</span><span class="sxs-lookup"><span data-stu-id="6930f-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6930f-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6930f-130">JSON Representation</span></span>
<span data-ttu-id="6930f-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6930f-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterStatusDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterStatusDetails",
  "managedDeviceId": "String",
  "payloadId": "String",
  "userId": "String",
  "deviceProperties": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "evalutionSummaries": [
    {
      "@odata.type": "microsoft.graph.assignmentFilterEvaluationSummary",
      "assignmentFilterId": "String",
      "assignmentFilterLastModifiedDateTime": "String (timestamp)",
      "assignmentFilterDisplayName": "String",
      "assignmentFilterPlatform": "String",
      "evaluationResult": "String",
      "evaluationDateTime": "String (timestamp)",
      "assignmentFilterType": "String"
    }
  ]
}
```




