---
title: Тип ресурса Усерекспериенцеаналитиксинсигхт
description: Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b5a712766534793fd11ba8b07955870d7e1195dd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43389247"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a><span data-ttu-id="22fa5-103">Тип ресурса Усерекспериенцеаналитиксинсигхт</span><span class="sxs-lookup"><span data-stu-id="22fa5-103">userExperienceAnalyticsInsight resource type</span></span>

<span data-ttu-id="22fa5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22fa5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22fa5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22fa5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22fa5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22fa5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22fa5-107">Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="22fa5-107">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="22fa5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="22fa5-108">Properties</span></span>
|<span data-ttu-id="22fa5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="22fa5-109">Property</span></span>|<span data-ttu-id="22fa5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="22fa5-110">Type</span></span>|<span data-ttu-id="22fa5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="22fa5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22fa5-112">усерекспериенцеаналитиксметриЦид</span><span class="sxs-lookup"><span data-stu-id="22fa5-112">userExperienceAnalyticsMetricId</span></span>|<span data-ttu-id="22fa5-113">String</span><span class="sxs-lookup"><span data-stu-id="22fa5-113">String</span></span>|<span data-ttu-id="22fa5-114">Уникальный идентификатор аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="22fa5-114">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="22fa5-115">инсигхтид</span><span class="sxs-lookup"><span data-stu-id="22fa5-115">insightId</span></span>|<span data-ttu-id="22fa5-116">String</span><span class="sxs-lookup"><span data-stu-id="22fa5-116">String</span></span>|<span data-ttu-id="22fa5-117">Уникальный идентификатор аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="22fa5-117">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="22fa5-118">values</span><span class="sxs-lookup"><span data-stu-id="22fa5-118">values</span></span>|<span data-ttu-id="22fa5-119">Коллекция [усерекспериенцеаналитиксинсигхтвалуе](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)</span><span class="sxs-lookup"><span data-stu-id="22fa5-119">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md) collection</span></span>|<span data-ttu-id="22fa5-120">Значение аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="22fa5-120">The value of the user experience analytics insight.</span></span>|
|<span data-ttu-id="22fa5-121">severity</span><span class="sxs-lookup"><span data-stu-id="22fa5-121">severity</span></span>|[<span data-ttu-id="22fa5-122">userExperienceAnalyticsInsightSeverity</span><span class="sxs-lookup"><span data-stu-id="22fa5-122">userExperienceAnalyticsInsightSeverity</span></span>](../resources/intune-devices-userexperienceanalyticsinsightseverity.md)|<span data-ttu-id="22fa5-123">Значение аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="22fa5-123">The value of the user experience analytics insight.</span></span> <span data-ttu-id="22fa5-124">Возможные значения: `none`, `informational`, `warning`, `error`.</span><span class="sxs-lookup"><span data-stu-id="22fa5-124">Possible values are: `none`, `informational`, `warning`, `error`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22fa5-125">Связи</span><span class="sxs-lookup"><span data-stu-id="22fa5-125">Relationships</span></span>
<span data-ttu-id="22fa5-126">Нет</span><span class="sxs-lookup"><span data-stu-id="22fa5-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22fa5-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="22fa5-127">JSON Representation</span></span>
<span data-ttu-id="22fa5-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22fa5-128">Here is a JSON representation of the resource.</span></span>
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



