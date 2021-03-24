---
title: тип ресурса userExperienceAnalyticsCategory
description: Объект аналитики пользовательского опыта содержит оценки и сведения о различных метриках категории.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f138b2417bccd6ed089810335e375eb721af80c6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141444"
---
# <a name="userexperienceanalyticscategory-resource-type"></a><span data-ttu-id="cc69e-103">тип ресурса userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="cc69e-103">userExperienceAnalyticsCategory resource type</span></span>

<span data-ttu-id="cc69e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc69e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc69e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc69e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc69e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc69e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc69e-107">Объект аналитики пользовательского опыта содержит оценки и сведения о различных метриках категории.</span><span class="sxs-lookup"><span data-stu-id="cc69e-107">The user experience analytics category entity contains the scores and insights for the various metrics of a category.</span></span>

## <a name="methods"></a><span data-ttu-id="cc69e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="cc69e-108">Methods</span></span>
|<span data-ttu-id="cc69e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="cc69e-109">Method</span></span>|<span data-ttu-id="cc69e-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cc69e-110">Return Type</span></span>|<span data-ttu-id="cc69e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cc69e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cc69e-112">Get userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="cc69e-112">Get userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-get.md)|[<span data-ttu-id="cc69e-113">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="cc69e-113">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="cc69e-114">Чтение свойств и связей [объекта userExperienceAnalyticsCategory.](../resources/intune-devices-userexperienceanalyticscategory.md)</span><span class="sxs-lookup"><span data-stu-id="cc69e-114">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|
|[<span data-ttu-id="cc69e-115">Обновление userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="cc69e-115">Update userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-update.md)|[<span data-ttu-id="cc69e-116">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="cc69e-116">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="cc69e-117">Обновление свойств объекта [userExperienceAnalyticsCategory.](../resources/intune-devices-userexperienceanalyticscategory.md)</span><span class="sxs-lookup"><span data-stu-id="cc69e-117">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cc69e-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc69e-118">Properties</span></span>
|<span data-ttu-id="cc69e-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc69e-119">Property</span></span>|<span data-ttu-id="cc69e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="cc69e-120">Type</span></span>|<span data-ttu-id="cc69e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cc69e-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc69e-122">id</span><span class="sxs-lookup"><span data-stu-id="cc69e-122">id</span></span>|<span data-ttu-id="cc69e-123">Строка</span><span class="sxs-lookup"><span data-stu-id="cc69e-123">String</span></span>|<span data-ttu-id="cc69e-124">Уникальный идентификатор категории аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="cc69e-124">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="cc69e-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="cc69e-125">overallScore</span></span>|<span data-ttu-id="cc69e-126">Int32</span><span class="sxs-lookup"><span data-stu-id="cc69e-126">Int32</span></span>|<span data-ttu-id="cc69e-127">Общая оценка категории аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="cc69e-127">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="cc69e-128">totalDevices</span><span class="sxs-lookup"><span data-stu-id="cc69e-128">totalDevices</span></span>|<span data-ttu-id="cc69e-129">Int32</span><span class="sxs-lookup"><span data-stu-id="cc69e-129">Int32</span></span>|<span data-ttu-id="cc69e-130">Общее число устройств категории аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="cc69e-130">The total device count of the user experience analytics category.</span></span>|
|<span data-ttu-id="cc69e-131">insights</span><span class="sxs-lookup"><span data-stu-id="cc69e-131">insights</span></span>|<span data-ttu-id="cc69e-132">[коллекция userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="cc69e-132">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="cc69e-133">Сведения о категории аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="cc69e-133">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="cc69e-134">state</span><span class="sxs-lookup"><span data-stu-id="cc69e-134">state</span></span>|[<span data-ttu-id="cc69e-135">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="cc69e-135">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="cc69e-136">Текущее состояние здоровья категории аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="cc69e-136">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="cc69e-137">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="cc69e-137">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc69e-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="cc69e-138">Relationships</span></span>
|<span data-ttu-id="cc69e-139">Связь</span><span class="sxs-lookup"><span data-stu-id="cc69e-139">Relationship</span></span>|<span data-ttu-id="cc69e-140">Тип</span><span class="sxs-lookup"><span data-stu-id="cc69e-140">Type</span></span>|<span data-ttu-id="cc69e-141">Описание</span><span class="sxs-lookup"><span data-stu-id="cc69e-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc69e-142">metricValues</span><span class="sxs-lookup"><span data-stu-id="cc69e-142">metricValues</span></span>|<span data-ttu-id="cc69e-143">[коллекция userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)</span><span class="sxs-lookup"><span data-stu-id="cc69e-143">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) collection</span></span>|<span data-ttu-id="cc69e-144">Метрические значения для категории аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="cc69e-144">The metric values for the user experience analytics category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc69e-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc69e-145">JSON Representation</span></span>
<span data-ttu-id="cc69e-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc69e-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "String (identifier)",
  "overallScore": 1024,
  "totalDevices": 1024,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
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
  ],
  "state": "String"
}
```




