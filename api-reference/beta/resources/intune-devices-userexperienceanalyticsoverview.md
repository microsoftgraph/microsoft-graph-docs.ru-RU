---
title: Тип ресурса Усерекспериенцеаналитиксовервиев
description: В объекте обзор анализа взаимодействия с пользователем содержатся общие показатели и оценки всех показателей всех категорий.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 306c6c9e2ca1903c2bd16012dba3b78e1c906cd6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783769"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="9b419-103">Тип ресурса Усерекспериенцеаналитиксовервиев</span><span class="sxs-lookup"><span data-stu-id="9b419-103">userExperienceAnalyticsOverview resource type</span></span>

> <span data-ttu-id="9b419-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b419-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b419-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b419-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b419-106">В объекте обзор анализа взаимодействия с пользователем содержатся общие показатели и оценки всех показателей всех категорий.</span><span class="sxs-lookup"><span data-stu-id="9b419-106">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="9b419-107">Методы</span><span class="sxs-lookup"><span data-stu-id="9b419-107">Methods</span></span>
|<span data-ttu-id="9b419-108">Метод</span><span class="sxs-lookup"><span data-stu-id="9b419-108">Method</span></span>|<span data-ttu-id="9b419-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9b419-109">Return Type</span></span>|<span data-ttu-id="9b419-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9b419-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9b419-111">Получение Усерекспериенцеаналитиксовервиев</span><span class="sxs-lookup"><span data-stu-id="9b419-111">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="9b419-112">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="9b419-112">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="9b419-113">Чтение свойств и связей объекта [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="9b419-113">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="9b419-114">Обновление Усерекспериенцеаналитиксовервиев</span><span class="sxs-lookup"><span data-stu-id="9b419-114">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="9b419-115">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="9b419-115">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="9b419-116">Обновление свойств объекта [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="9b419-116">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9b419-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b419-117">Properties</span></span>
|<span data-ttu-id="9b419-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b419-118">Property</span></span>|<span data-ttu-id="9b419-119">Тип</span><span class="sxs-lookup"><span data-stu-id="9b419-119">Type</span></span>|<span data-ttu-id="9b419-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9b419-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b419-121">id</span><span class="sxs-lookup"><span data-stu-id="9b419-121">id</span></span>|<span data-ttu-id="9b419-122">String</span><span class="sxs-lookup"><span data-stu-id="9b419-122">String</span></span>|<span data-ttu-id="9b419-123">Уникальный идентификатор для обзора аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="9b419-123">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="9b419-124">овераллскоре</span><span class="sxs-lookup"><span data-stu-id="9b419-124">overallScore</span></span>|<span data-ttu-id="9b419-125">Int32</span><span class="sxs-lookup"><span data-stu-id="9b419-125">Int32</span></span>|<span data-ttu-id="9b419-126">Общий показатель аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="9b419-126">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="9b419-127">девицебутперформанцеовераллскоре</span><span class="sxs-lookup"><span data-stu-id="9b419-127">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="9b419-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9b419-128">Int32</span></span>|<span data-ttu-id="9b419-129">Общая оценка производительности при загрузке устройства Analytics.</span><span class="sxs-lookup"><span data-stu-id="9b419-129">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="9b419-130">бестпрактицесовераллскоре</span><span class="sxs-lookup"><span data-stu-id="9b419-130">bestPracticesOverallScore</span></span>|<span data-ttu-id="9b419-131">Int32</span><span class="sxs-lookup"><span data-stu-id="9b419-131">Int32</span></span>|<span data-ttu-id="9b419-132">Общая оценка рекомендаций по анализу пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="9b419-132">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="9b419-133">insights</span><span class="sxs-lookup"><span data-stu-id="9b419-133">insights</span></span>|<span data-ttu-id="9b419-134">Коллекция [усерекспериенцеаналитиксинсигхт](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="9b419-134">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="9b419-135">Аналитика взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="9b419-135">The user experience analytics insights.</span></span>|
|<span data-ttu-id="9b419-136">state</span><span class="sxs-lookup"><span data-stu-id="9b419-136">state</span></span>|[<span data-ttu-id="9b419-137">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="9b419-137">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="9b419-138">Текущее состояние работоспособности в обзоре аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="9b419-138">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="9b419-139">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="9b419-139">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="9b419-140">девицебутперформанцехеалсстате</span><span class="sxs-lookup"><span data-stu-id="9b419-140">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="9b419-141">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="9b419-141">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="9b419-142">Текущее состояние работоспособности категории аналитики взаимодействия с пользователем "Бутперформанце".</span><span class="sxs-lookup"><span data-stu-id="9b419-142">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="9b419-143">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="9b419-143">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="9b419-144">бестпрактицешеалсстате</span><span class="sxs-lookup"><span data-stu-id="9b419-144">bestPracticesHealthState</span></span>|[<span data-ttu-id="9b419-145">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="9b419-145">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="9b419-146">Текущее состояние работоспособности категории аналитики взаимодействия с пользователем "Бестпрактицес".</span><span class="sxs-lookup"><span data-stu-id="9b419-146">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="9b419-147">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="9b419-147">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b419-148">Связи</span><span class="sxs-lookup"><span data-stu-id="9b419-148">Relationships</span></span>
<span data-ttu-id="9b419-149">Нет</span><span class="sxs-lookup"><span data-stu-id="9b419-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b419-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b419-150">JSON Representation</span></span>
<span data-ttu-id="9b419-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b419-151">Here is a JSON representation of the resource.</span></span>
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
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
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
  ],
  "state": "String",
  "deviceBootPerformanceHealthState": "String",
  "bestPracticesHealthState": "String"
}
```



