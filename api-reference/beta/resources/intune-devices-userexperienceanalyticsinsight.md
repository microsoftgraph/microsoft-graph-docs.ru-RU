---
title: Тип ресурса Усерекспериенцеаналитиксинсигхт
description: Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c28df3bc40f02948198a67850de6fd573607a366
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783797"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a><span data-ttu-id="9e054-103">Тип ресурса Усерекспериенцеаналитиксинсигхт</span><span class="sxs-lookup"><span data-stu-id="9e054-103">userExperienceAnalyticsInsight resource type</span></span>

> <span data-ttu-id="9e054-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e054-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e054-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9e054-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e054-106">Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="9e054-106">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="9e054-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e054-107">Properties</span></span>
|<span data-ttu-id="9e054-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e054-108">Property</span></span>|<span data-ttu-id="9e054-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9e054-109">Type</span></span>|<span data-ttu-id="9e054-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9e054-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e054-111">усерекспериенцеаналитиксметриЦид</span><span class="sxs-lookup"><span data-stu-id="9e054-111">userExperienceAnalyticsMetricId</span></span>|<span data-ttu-id="9e054-112">String</span><span class="sxs-lookup"><span data-stu-id="9e054-112">String</span></span>|<span data-ttu-id="9e054-113">Уникальный идентификатор аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="9e054-113">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="9e054-114">инсигхтид</span><span class="sxs-lookup"><span data-stu-id="9e054-114">insightId</span></span>|<span data-ttu-id="9e054-115">String</span><span class="sxs-lookup"><span data-stu-id="9e054-115">String</span></span>|<span data-ttu-id="9e054-116">Уникальный идентификатор аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="9e054-116">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="9e054-117">values</span><span class="sxs-lookup"><span data-stu-id="9e054-117">values</span></span>|<span data-ttu-id="9e054-118">Коллекция [усерекспериенцеаналитиксинсигхтвалуе](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9e054-118">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md) collection</span></span>|<span data-ttu-id="9e054-119">Значение аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="9e054-119">The value of the user experience analytics insight.</span></span>|
|<span data-ttu-id="9e054-120">severity</span><span class="sxs-lookup"><span data-stu-id="9e054-120">severity</span></span>|[<span data-ttu-id="9e054-121">userExperienceAnalyticsInsightSeverity</span><span class="sxs-lookup"><span data-stu-id="9e054-121">userExperienceAnalyticsInsightSeverity</span></span>](../resources/intune-devices-userexperienceanalyticsinsightseverity.md)|<span data-ttu-id="9e054-122">Значение аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="9e054-122">The value of the user experience analytics insight.</span></span> <span data-ttu-id="9e054-123">Возможные значения: `none`, `informational`, `warning`, `error`.</span><span class="sxs-lookup"><span data-stu-id="9e054-123">Possible values are: `none`, `informational`, `warning`, `error`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e054-124">Связи</span><span class="sxs-lookup"><span data-stu-id="9e054-124">Relationships</span></span>
<span data-ttu-id="9e054-125">Нет</span><span class="sxs-lookup"><span data-stu-id="9e054-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e054-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9e054-126">JSON Representation</span></span>
<span data-ttu-id="9e054-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e054-127">Here is a JSON representation of the resource.</span></span>
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



