---
title: тип ресурса userExperienceAnalyticsOverview
description: Объект аналитики пользовательских интерфейсов содержит общую оценку, оценки и сведения по каждой метрике всех категорий.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d05f29a375bf69a31bfb27805a2f698da673bc12
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159314"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="eef8b-103">тип ресурса userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="eef8b-103">userExperienceAnalyticsOverview resource type</span></span>

<span data-ttu-id="eef8b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eef8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eef8b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eef8b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eef8b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eef8b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eef8b-107">Объект аналитики пользовательских интерфейсов содержит общую оценку, оценки и сведения по каждой метрике всех категорий.</span><span class="sxs-lookup"><span data-stu-id="eef8b-107">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="eef8b-108">Методы</span><span class="sxs-lookup"><span data-stu-id="eef8b-108">Methods</span></span>
|<span data-ttu-id="eef8b-109">Метод</span><span class="sxs-lookup"><span data-stu-id="eef8b-109">Method</span></span>|<span data-ttu-id="eef8b-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eef8b-110">Return Type</span></span>|<span data-ttu-id="eef8b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eef8b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eef8b-112">Get userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="eef8b-112">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="eef8b-113">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="eef8b-113">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="eef8b-114">Чтение свойств и связей [объекта userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="eef8b-114">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="eef8b-115">Обновление userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="eef8b-115">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="eef8b-116">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="eef8b-116">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="eef8b-117">Обновление свойств объекта [userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="eef8b-117">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="eef8b-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="eef8b-118">Properties</span></span>
|<span data-ttu-id="eef8b-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="eef8b-119">Property</span></span>|<span data-ttu-id="eef8b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="eef8b-120">Type</span></span>|<span data-ttu-id="eef8b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="eef8b-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eef8b-122">id</span><span class="sxs-lookup"><span data-stu-id="eef8b-122">id</span></span>|<span data-ttu-id="eef8b-123">Строка</span><span class="sxs-lookup"><span data-stu-id="eef8b-123">String</span></span>|<span data-ttu-id="eef8b-124">Уникальный идентификатор обзора аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="eef8b-124">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="eef8b-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="eef8b-125">overallScore</span></span>|<span data-ttu-id="eef8b-126">Int32</span><span class="sxs-lookup"><span data-stu-id="eef8b-126">Int32</span></span>|<span data-ttu-id="eef8b-127">Общая оценка аналитики пользовательского опыта.</span><span class="sxs-lookup"><span data-stu-id="eef8b-127">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="eef8b-128">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="eef8b-128">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="eef8b-129">Int32</span><span class="sxs-lookup"><span data-stu-id="eef8b-129">Int32</span></span>|<span data-ttu-id="eef8b-130">Общая оценка производительности загрузки устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="eef8b-130">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="eef8b-131">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="eef8b-131">bestPracticesOverallScore</span></span>|<span data-ttu-id="eef8b-132">Int32</span><span class="sxs-lookup"><span data-stu-id="eef8b-132">Int32</span></span>|<span data-ttu-id="eef8b-133">Анализ пользовательских интерфейсов позволяет опытом работы с общим показателем.</span><span class="sxs-lookup"><span data-stu-id="eef8b-133">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="eef8b-134">workFromAnywhereOverallScore</span><span class="sxs-lookup"><span data-stu-id="eef8b-134">workFromAnywhereOverallScore</span></span>|<span data-ttu-id="eef8b-135">Int32</span><span class="sxs-lookup"><span data-stu-id="eef8b-135">Int32</span></span>|<span data-ttu-id="eef8b-136">Аналитика пользовательского интерфейса Работает с любого общего балла.</span><span class="sxs-lookup"><span data-stu-id="eef8b-136">The user experience analytics Work From Anywhere overall score.</span></span>|
|<span data-ttu-id="eef8b-137">appHealthOverallScore</span><span class="sxs-lookup"><span data-stu-id="eef8b-137">appHealthOverallScore</span></span>|<span data-ttu-id="eef8b-138">Int32</span><span class="sxs-lookup"><span data-stu-id="eef8b-138">Int32</span></span>|<span data-ttu-id="eef8b-139">Общее состояние здоровья приложения для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="eef8b-139">The user experience analytics app health overall score.</span></span>|
|<span data-ttu-id="eef8b-140">resourcePerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="eef8b-140">resourcePerformanceOverallScore</span></span>|<span data-ttu-id="eef8b-141">Int32</span><span class="sxs-lookup"><span data-stu-id="eef8b-141">Int32</span></span>|<span data-ttu-id="eef8b-142">Общая оценка производительности ресурсов аналитики пользовательских ресурсов.</span><span class="sxs-lookup"><span data-stu-id="eef8b-142">The user experience analytics resource performance overall score.</span></span>|
|<span data-ttu-id="eef8b-143">insights</span><span class="sxs-lookup"><span data-stu-id="eef8b-143">insights</span></span>|<span data-ttu-id="eef8b-144">[коллекция userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="eef8b-144">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="eef8b-145">Аналитические сведения о пользовательском опыте.</span><span class="sxs-lookup"><span data-stu-id="eef8b-145">The user experience analytics insights.</span></span>|
|<span data-ttu-id="eef8b-146">state</span><span class="sxs-lookup"><span data-stu-id="eef8b-146">state</span></span>|[<span data-ttu-id="eef8b-147">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="eef8b-147">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="eef8b-148">Текущее состояние состояния состояния аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="eef8b-148">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="eef8b-149">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="eef8b-149">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="eef8b-150">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="eef8b-150">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="eef8b-151">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="eef8b-151">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="eef8b-152">Текущее состояние состояния состояния аналитики пользовательского интерфейса категории BootPerformance.</span><span class="sxs-lookup"><span data-stu-id="eef8b-152">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="eef8b-153">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="eef8b-153">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="eef8b-154">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="eef8b-154">bestPracticesHealthState</span></span>|[<span data-ttu-id="eef8b-155">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="eef8b-155">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="eef8b-156">Текущее состояние здоровья категории аналитики пользовательских интерфейсов "BestPractices".</span><span class="sxs-lookup"><span data-stu-id="eef8b-156">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="eef8b-157">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="eef8b-157">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="eef8b-158">workFromAnywhereHealthState</span><span class="sxs-lookup"><span data-stu-id="eef8b-158">workFromAnywhereHealthState</span></span>|[<span data-ttu-id="eef8b-159">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="eef8b-159">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="eef8b-160">Текущее состояние состояния здоровья аналитики пользовательских интерфейсов категории WorkFromAnywhere.</span><span class="sxs-lookup"><span data-stu-id="eef8b-160">The current health state of the user experience analytics 'WorkFromAnywhere' category.</span></span> <span data-ttu-id="eef8b-161">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="eef8b-161">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="eef8b-162">appHealthState</span><span class="sxs-lookup"><span data-stu-id="eef8b-162">appHealthState</span></span>|[<span data-ttu-id="eef8b-163">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="eef8b-163">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="eef8b-164">Текущее состояние здоровья категории аналитики пользовательских интерфейсов "BestPractices".</span><span class="sxs-lookup"><span data-stu-id="eef8b-164">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="eef8b-165">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="eef8b-165">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="eef8b-166">resourcePerformanceState</span><span class="sxs-lookup"><span data-stu-id="eef8b-166">resourcePerformanceState</span></span>|[<span data-ttu-id="eef8b-167">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="eef8b-167">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="eef8b-168">Текущее состояние состояния здоровья в категории аналитики пользовательского интерфейса "ResourcePerformance".</span><span class="sxs-lookup"><span data-stu-id="eef8b-168">The current health state of the user experience analytics 'ResourcePerformance' category.</span></span> <span data-ttu-id="eef8b-169">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="eef8b-169">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eef8b-170">Отношения</span><span class="sxs-lookup"><span data-stu-id="eef8b-170">Relationships</span></span>
<span data-ttu-id="eef8b-171">Нет</span><span class="sxs-lookup"><span data-stu-id="eef8b-171">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eef8b-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eef8b-172">JSON Representation</span></span>
<span data-ttu-id="eef8b-173">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eef8b-173">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "String (identifier)",
  "overallScore": 1024,
  "deviceBootPerformanceOverallScore": 1024,
  "bestPracticesOverallScore": 1024,
  "workFromAnywhereOverallScore": 1024,
  "appHealthOverallScore": 1024,
  "resourcePerformanceOverallScore": 1024,
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
  "state": "String",
  "deviceBootPerformanceHealthState": "String",
  "bestPracticesHealthState": "String",
  "workFromAnywhereHealthState": "String",
  "appHealthState": "String",
  "resourcePerformanceState": "String"
}
```




