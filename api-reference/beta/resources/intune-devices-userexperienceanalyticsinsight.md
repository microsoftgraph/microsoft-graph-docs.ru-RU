---
title: Тип ресурса Усерекспериенцеаналитиксинсигхт
description: Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 40e82f0c950328c0a6937a38762c6a26344fb943
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178817"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a><span data-ttu-id="0d4f1-103">Тип ресурса Усерекспериенцеаналитиксинсигхт</span><span class="sxs-lookup"><span data-stu-id="0d4f1-103">userExperienceAnalyticsInsight resource type</span></span>

<span data-ttu-id="0d4f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d4f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d4f1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d4f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d4f1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d4f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d4f1-107">Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="0d4f1-107">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="0d4f1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d4f1-108">Properties</span></span>
|<span data-ttu-id="0d4f1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d4f1-109">Property</span></span>|<span data-ttu-id="0d4f1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0d4f1-110">Type</span></span>|<span data-ttu-id="0d4f1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0d4f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d4f1-112">усерекспериенцеаналитиксметриЦид</span><span class="sxs-lookup"><span data-stu-id="0d4f1-112">userExperienceAnalyticsMetricId</span></span>|<span data-ttu-id="0d4f1-113">Строка</span><span class="sxs-lookup"><span data-stu-id="0d4f1-113">String</span></span>|<span data-ttu-id="0d4f1-114">Уникальный идентификатор аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d4f1-114">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="0d4f1-115">инсигхтид</span><span class="sxs-lookup"><span data-stu-id="0d4f1-115">insightId</span></span>|<span data-ttu-id="0d4f1-116">Строка</span><span class="sxs-lookup"><span data-stu-id="0d4f1-116">String</span></span>|<span data-ttu-id="0d4f1-117">Уникальный идентификатор аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d4f1-117">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="0d4f1-118">values</span><span class="sxs-lookup"><span data-stu-id="0d4f1-118">values</span></span>|<span data-ttu-id="0d4f1-119">Коллекция [усерекспериенцеаналитиксинсигхтвалуе](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)</span><span class="sxs-lookup"><span data-stu-id="0d4f1-119">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md) collection</span></span>|<span data-ttu-id="0d4f1-120">Значение аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d4f1-120">The value of the user experience analytics insight.</span></span>|
|<span data-ttu-id="0d4f1-121">severity</span><span class="sxs-lookup"><span data-stu-id="0d4f1-121">severity</span></span>|[<span data-ttu-id="0d4f1-122">userExperienceAnalyticsInsightSeverity</span><span class="sxs-lookup"><span data-stu-id="0d4f1-122">userExperienceAnalyticsInsightSeverity</span></span>](../resources/intune-devices-userexperienceanalyticsinsightseverity.md)|<span data-ttu-id="0d4f1-123">Значение аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d4f1-123">The value of the user experience analytics insight.</span></span> <span data-ttu-id="0d4f1-124">Возможные значения: `none`, `informational`, `warning`, `error`.</span><span class="sxs-lookup"><span data-stu-id="0d4f1-124">Possible values are: `none`, `informational`, `warning`, `error`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d4f1-125">Связи</span><span class="sxs-lookup"><span data-stu-id="0d4f1-125">Relationships</span></span>
<span data-ttu-id="0d4f1-126">Нет</span><span class="sxs-lookup"><span data-stu-id="0d4f1-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d4f1-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d4f1-127">JSON Representation</span></span>
<span data-ttu-id="0d4f1-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d4f1-128">Here is a JSON representation of the resource.</span></span>
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



