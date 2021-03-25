---
title: тип ресурса assignmentFilterStatusDetails
description: Представляем сведения о состоянии для устройства и полезной нагрузки и всех связанных с ними прикладных фильтров.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: be36fae74e412395bd74a24b11b36b48cbf165ff
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155976"
---
# <a name="assignmentfilterstatusdetails-resource-type"></a><span data-ttu-id="37409-103">тип ресурса assignmentFilterStatusDetails</span><span class="sxs-lookup"><span data-stu-id="37409-103">assignmentFilterStatusDetails resource type</span></span>

<span data-ttu-id="37409-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37409-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37409-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37409-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37409-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37409-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37409-107">Представляем сведения о состоянии для устройства и полезной нагрузки и всех связанных с ними прикладных фильтров.</span><span class="sxs-lookup"><span data-stu-id="37409-107">Represent status details for device and payload and all associated applied filters.</span></span>

## <a name="properties"></a><span data-ttu-id="37409-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="37409-108">Properties</span></span>
|<span data-ttu-id="37409-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="37409-109">Property</span></span>|<span data-ttu-id="37409-110">Тип</span><span class="sxs-lookup"><span data-stu-id="37409-110">Type</span></span>|<span data-ttu-id="37409-111">Описание</span><span class="sxs-lookup"><span data-stu-id="37409-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37409-112">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="37409-112">managedDeviceId</span></span>|<span data-ttu-id="37409-113">Строка</span><span class="sxs-lookup"><span data-stu-id="37409-113">String</span></span>|<span data-ttu-id="37409-114">Уникальный идентификатор для объекта устройства.</span><span class="sxs-lookup"><span data-stu-id="37409-114">Unique identifier for the device object.</span></span>|
|<span data-ttu-id="37409-115">payloadId</span><span class="sxs-lookup"><span data-stu-id="37409-115">payloadId</span></span>|<span data-ttu-id="37409-116">Строка</span><span class="sxs-lookup"><span data-stu-id="37409-116">String</span></span>|<span data-ttu-id="37409-117">Уникальный идентификатор для объекта полезной нагрузки.</span><span class="sxs-lookup"><span data-stu-id="37409-117">Unique identifier for payload object.</span></span>|
|<span data-ttu-id="37409-118">userId</span><span class="sxs-lookup"><span data-stu-id="37409-118">userId</span></span>|<span data-ttu-id="37409-119">String</span><span class="sxs-lookup"><span data-stu-id="37409-119">String</span></span>|<span data-ttu-id="37409-120">Уникальный идентификатор для объекта UserId.</span><span class="sxs-lookup"><span data-stu-id="37409-120">Unique identifier for UserId object.</span></span> <span data-ttu-id="37409-121">Может быть null</span><span class="sxs-lookup"><span data-stu-id="37409-121">Can be null</span></span>|
|<span data-ttu-id="37409-122">свойства устройств</span><span class="sxs-lookup"><span data-stu-id="37409-122">deviceProperties</span></span>|<span data-ttu-id="37409-123">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="37409-123">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="37409-124">Свойства устройства, используемые для оценки фильтра во время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="37409-124">Device properties used for filter evaluation during device check-in time.</span></span>|
|<span data-ttu-id="37409-125">evalutionSummaries</span><span class="sxs-lookup"><span data-stu-id="37409-125">evalutionSummaries</span></span>|<span data-ttu-id="37409-126">[assignmentFilterEvaluationSummary](../resources/intune-policyset-assignmentfilterevaluationsummary.md) collection</span><span class="sxs-lookup"><span data-stu-id="37409-126">[assignmentFilterEvaluationSummary](../resources/intune-policyset-assignmentfilterevaluationsummary.md) collection</span></span>|<span data-ttu-id="37409-127">Сводки результатов оценки для каждого фильтра, связанного с устройством и полезной нагрузкой</span><span class="sxs-lookup"><span data-stu-id="37409-127">Evaluation result summaries for each filter associated to device and payload</span></span>|

## <a name="relationships"></a><span data-ttu-id="37409-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="37409-128">Relationships</span></span>
<span data-ttu-id="37409-129">Нет</span><span class="sxs-lookup"><span data-stu-id="37409-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37409-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37409-130">JSON Representation</span></span>
<span data-ttu-id="37409-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37409-131">Here is a JSON representation of the resource.</span></span>
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
      "assignmentFilterType": "String",
      "assignmentFilterTypeAndEvaluationResults": [
        {
          "@odata.type": "microsoft.graph.assignmentFilterTypeAndEvaluationResult",
          "assignmentFilterType": "String",
          "evaluationResult": "String"
        }
      ]
    }
  ]
}
```




