---
title: Тип ресурса Усерекспериенцеаналитиксинсигхт
description: Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3cd10bef08119c3ec123bad14a2274c5ec40fc3b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724412"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a><span data-ttu-id="d7ab2-103">Тип ресурса Усерекспериенцеаналитиксинсигхт</span><span class="sxs-lookup"><span data-stu-id="d7ab2-103">userExperienceAnalyticsInsight resource type</span></span>

<span data-ttu-id="d7ab2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7ab2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7ab2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7ab2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7ab2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7ab2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7ab2-107">Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="d7ab2-107">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="d7ab2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7ab2-108">Properties</span></span>
|<span data-ttu-id="d7ab2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7ab2-109">Property</span></span>|<span data-ttu-id="d7ab2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d7ab2-110">Type</span></span>|<span data-ttu-id="d7ab2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d7ab2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7ab2-112">усерекспериенцеаналитиксметриЦид</span><span class="sxs-lookup"><span data-stu-id="d7ab2-112">userExperienceAnalyticsMetricId</span></span>|<span data-ttu-id="d7ab2-113">Строка</span><span class="sxs-lookup"><span data-stu-id="d7ab2-113">String</span></span>|<span data-ttu-id="d7ab2-114">Уникальный идентификатор аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="d7ab2-114">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="d7ab2-115">инсигхтид</span><span class="sxs-lookup"><span data-stu-id="d7ab2-115">insightId</span></span>|<span data-ttu-id="d7ab2-116">Строка</span><span class="sxs-lookup"><span data-stu-id="d7ab2-116">String</span></span>|<span data-ttu-id="d7ab2-117">Уникальный идентификатор аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="d7ab2-117">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="d7ab2-118">values</span><span class="sxs-lookup"><span data-stu-id="d7ab2-118">values</span></span>|<span data-ttu-id="d7ab2-119">Коллекция [усерекспериенцеаналитиксинсигхтвалуе](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d7ab2-119">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md) collection</span></span>|<span data-ttu-id="d7ab2-120">Значение аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="d7ab2-120">The value of the user experience analytics insight.</span></span>|
|<span data-ttu-id="d7ab2-121">severity</span><span class="sxs-lookup"><span data-stu-id="d7ab2-121">severity</span></span>|[<span data-ttu-id="d7ab2-122">userExperienceAnalyticsInsightSeverity</span><span class="sxs-lookup"><span data-stu-id="d7ab2-122">userExperienceAnalyticsInsightSeverity</span></span>](../resources/intune-devices-userexperienceanalyticsinsightseverity.md)|<span data-ttu-id="d7ab2-123">Значение аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="d7ab2-123">The value of the user experience analytics insight.</span></span> <span data-ttu-id="d7ab2-124">Возможные значения: `none`, `informational`, `warning`, `error`.</span><span class="sxs-lookup"><span data-stu-id="d7ab2-124">Possible values are: `none`, `informational`, `warning`, `error`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7ab2-125">Связи</span><span class="sxs-lookup"><span data-stu-id="d7ab2-125">Relationships</span></span>
<span data-ttu-id="d7ab2-126">Нет</span><span class="sxs-lookup"><span data-stu-id="d7ab2-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7ab2-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7ab2-127">JSON Representation</span></span>
<span data-ttu-id="d7ab2-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7ab2-128">Here is a JSON representation of the resource.</span></span>
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
      "value": "4.2"
    }
  ],
  "severity": "String"
}
```





