---
title: Тип ресурса Усерекспериенцеаналитиксинсигхт
description: Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 70cb1e7405fdffcff0f1fd6a8a8361df6d941788
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196702"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a><span data-ttu-id="ba367-103">Тип ресурса Усерекспериенцеаналитиксинсигхт</span><span class="sxs-lookup"><span data-stu-id="ba367-103">userExperienceAnalyticsInsight resource type</span></span>

> <span data-ttu-id="ba367-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba367-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba367-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba367-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba367-106">Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="ba367-106">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="ba367-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba367-107">Properties</span></span>
|<span data-ttu-id="ba367-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba367-108">Property</span></span>|<span data-ttu-id="ba367-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ba367-109">Type</span></span>|<span data-ttu-id="ba367-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ba367-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba367-111">усерекспериенцеаналитиксметриЦид</span><span class="sxs-lookup"><span data-stu-id="ba367-111">userExperienceAnalyticsMetricId</span></span>|<span data-ttu-id="ba367-112">String.</span><span class="sxs-lookup"><span data-stu-id="ba367-112">String</span></span>|<span data-ttu-id="ba367-113">Уникальный идентификатор аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="ba367-113">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="ba367-114">инсигхтид</span><span class="sxs-lookup"><span data-stu-id="ba367-114">insightId</span></span>|<span data-ttu-id="ba367-115">String.</span><span class="sxs-lookup"><span data-stu-id="ba367-115">String</span></span>|<span data-ttu-id="ba367-116">Уникальный идентификатор аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="ba367-116">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="ba367-117">values</span><span class="sxs-lookup"><span data-stu-id="ba367-117">values</span></span>|<span data-ttu-id="ba367-118">Коллекция [усерекспериенцеаналитиксинсигхтвалуе](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)</span><span class="sxs-lookup"><span data-stu-id="ba367-118">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md) collection</span></span>|<span data-ttu-id="ba367-119">Значение аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="ba367-119">The value of the user experience analytics insight.</span></span>|
|<span data-ttu-id="ba367-120">severity</span><span class="sxs-lookup"><span data-stu-id="ba367-120">severity</span></span>|[<span data-ttu-id="ba367-121">усерекспериенцеаналитиксинсигхтсеверити</span><span class="sxs-lookup"><span data-stu-id="ba367-121">userExperienceAnalyticsInsightSeverity</span></span>](../resources/intune-devices-userexperienceanalyticsinsightseverity.md)|<span data-ttu-id="ba367-122">Значение аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="ba367-122">The value of the user experience analytics insight.</span></span> <span data-ttu-id="ba367-123">Возможные значения: `none`, `informational`, `warning`, `error`.</span><span class="sxs-lookup"><span data-stu-id="ba367-123">Possible values are: `none`, `informational`, `warning`, `error`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba367-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="ba367-124">Relationships</span></span>
<span data-ttu-id="ba367-125">Нет</span><span class="sxs-lookup"><span data-stu-id="ba367-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba367-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba367-126">JSON Representation</span></span>
<span data-ttu-id="ba367-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba367-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsInsight",
  "userExperienceAnalyticsMetricId": "String",
  "insightId": "String",
  "values": [
    {
      "@odata.type": "microsoft.graph.insightValueDouble",
      "value": "<Unknown Primitive Type Edm.Double>"
    }
  ],
  "severity": "String"
}
```



