---
title: Тип ресурса Усерекспериенцеаналитикскатегори
description: Сущность категории аналитики взаимодействия с пользователем содержит показатели и аналитические сведения о различных метриках категории.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2fabbc284745969c34a4495a7164007577c45750
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49208452"
---
# <a name="userexperienceanalyticscategory-resource-type"></a><span data-ttu-id="739ad-103">Тип ресурса Усерекспериенцеаналитикскатегори</span><span class="sxs-lookup"><span data-stu-id="739ad-103">userExperienceAnalyticsCategory resource type</span></span>

<span data-ttu-id="739ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="739ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="739ad-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="739ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="739ad-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="739ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="739ad-107">Сущность категории аналитики взаимодействия с пользователем содержит показатели и аналитические сведения о различных метриках категории.</span><span class="sxs-lookup"><span data-stu-id="739ad-107">The user experience analytics category entity contains the scores and insights for the various metrics of a category.</span></span>

## <a name="methods"></a><span data-ttu-id="739ad-108">Методы</span><span class="sxs-lookup"><span data-stu-id="739ad-108">Methods</span></span>
|<span data-ttu-id="739ad-109">Метод</span><span class="sxs-lookup"><span data-stu-id="739ad-109">Method</span></span>|<span data-ttu-id="739ad-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="739ad-110">Return Type</span></span>|<span data-ttu-id="739ad-111">Описание</span><span class="sxs-lookup"><span data-stu-id="739ad-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="739ad-112">Получение Усерекспериенцеаналитикскатегори</span><span class="sxs-lookup"><span data-stu-id="739ad-112">Get userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-get.md)|[<span data-ttu-id="739ad-113">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="739ad-113">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="739ad-114">Чтение свойств и связей объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="739ad-114">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|
|[<span data-ttu-id="739ad-115">Обновление Усерекспериенцеаналитикскатегори</span><span class="sxs-lookup"><span data-stu-id="739ad-115">Update userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-update.md)|[<span data-ttu-id="739ad-116">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="739ad-116">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="739ad-117">Обновление свойств объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="739ad-117">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="739ad-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="739ad-118">Properties</span></span>
|<span data-ttu-id="739ad-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="739ad-119">Property</span></span>|<span data-ttu-id="739ad-120">Тип</span><span class="sxs-lookup"><span data-stu-id="739ad-120">Type</span></span>|<span data-ttu-id="739ad-121">Описание</span><span class="sxs-lookup"><span data-stu-id="739ad-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="739ad-122">id</span><span class="sxs-lookup"><span data-stu-id="739ad-122">id</span></span>|<span data-ttu-id="739ad-123">String</span><span class="sxs-lookup"><span data-stu-id="739ad-123">String</span></span>|<span data-ttu-id="739ad-124">Уникальный идентификатор категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="739ad-124">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="739ad-125">овераллскоре</span><span class="sxs-lookup"><span data-stu-id="739ad-125">overallScore</span></span>|<span data-ttu-id="739ad-126">Int32</span><span class="sxs-lookup"><span data-stu-id="739ad-126">Int32</span></span>|<span data-ttu-id="739ad-127">Общий показатель категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="739ad-127">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="739ad-128">insights</span><span class="sxs-lookup"><span data-stu-id="739ad-128">insights</span></span>|<span data-ttu-id="739ad-129">Коллекция [усерекспериенцеаналитиксинсигхт](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="739ad-129">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="739ad-130">Аналитика для категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="739ad-130">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="739ad-131">state</span><span class="sxs-lookup"><span data-stu-id="739ad-131">state</span></span>|[<span data-ttu-id="739ad-132">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="739ad-132">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="739ad-133">Текущее состояние работоспособности категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="739ad-133">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="739ad-134">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="739ad-134">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="739ad-135">Связи</span><span class="sxs-lookup"><span data-stu-id="739ad-135">Relationships</span></span>
|<span data-ttu-id="739ad-136">Связь</span><span class="sxs-lookup"><span data-stu-id="739ad-136">Relationship</span></span>|<span data-ttu-id="739ad-137">Тип</span><span class="sxs-lookup"><span data-stu-id="739ad-137">Type</span></span>|<span data-ttu-id="739ad-138">Описание</span><span class="sxs-lookup"><span data-stu-id="739ad-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="739ad-139">метриквалуес</span><span class="sxs-lookup"><span data-stu-id="739ad-139">metricValues</span></span>|<span data-ttu-id="739ad-140">Коллекция [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md)</span><span class="sxs-lookup"><span data-stu-id="739ad-140">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) collection</span></span>|<span data-ttu-id="739ad-141">Значения метрик для категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="739ad-141">The metric values for the user experience analytics category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="739ad-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="739ad-142">JSON Representation</span></span>
<span data-ttu-id="739ad-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="739ad-143">Here is a JSON representation of the resource.</span></span>
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




