---
title: Тип ресурса Усерекспериенцеаналитикскатегори
description: Сущность категории аналитики взаимодействия с пользователем содержит показатели и аналитические сведения о различных метриках категории.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4ba9d56e1b20b66efe2b0653358dca4907ca0dc2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783839"
---
# <a name="userexperienceanalyticscategory-resource-type"></a><span data-ttu-id="0bb77-103">Тип ресурса Усерекспериенцеаналитикскатегори</span><span class="sxs-lookup"><span data-stu-id="0bb77-103">userExperienceAnalyticsCategory resource type</span></span>

> <span data-ttu-id="0bb77-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bb77-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bb77-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0bb77-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bb77-106">Сущность категории аналитики взаимодействия с пользователем содержит показатели и аналитические сведения о различных метриках категории.</span><span class="sxs-lookup"><span data-stu-id="0bb77-106">The user experience analytics category entity contains the scores and insights for the various metrics of a category.</span></span>

## <a name="methods"></a><span data-ttu-id="0bb77-107">Методы</span><span class="sxs-lookup"><span data-stu-id="0bb77-107">Methods</span></span>
|<span data-ttu-id="0bb77-108">Метод</span><span class="sxs-lookup"><span data-stu-id="0bb77-108">Method</span></span>|<span data-ttu-id="0bb77-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0bb77-109">Return Type</span></span>|<span data-ttu-id="0bb77-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0bb77-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0bb77-111">Получение Усерекспериенцеаналитикскатегори</span><span class="sxs-lookup"><span data-stu-id="0bb77-111">Get userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-get.md)|[<span data-ttu-id="0bb77-112">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="0bb77-112">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="0bb77-113">Чтение свойств и связей объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="0bb77-113">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|
|[<span data-ttu-id="0bb77-114">Обновление Усерекспериенцеаналитикскатегори</span><span class="sxs-lookup"><span data-stu-id="0bb77-114">Update userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-update.md)|[<span data-ttu-id="0bb77-115">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="0bb77-115">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="0bb77-116">Обновление свойств объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="0bb77-116">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0bb77-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="0bb77-117">Properties</span></span>
|<span data-ttu-id="0bb77-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="0bb77-118">Property</span></span>|<span data-ttu-id="0bb77-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0bb77-119">Type</span></span>|<span data-ttu-id="0bb77-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0bb77-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bb77-121">id</span><span class="sxs-lookup"><span data-stu-id="0bb77-121">id</span></span>|<span data-ttu-id="0bb77-122">String</span><span class="sxs-lookup"><span data-stu-id="0bb77-122">String</span></span>|<span data-ttu-id="0bb77-123">Уникальный идентификатор категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="0bb77-123">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="0bb77-124">овераллскоре</span><span class="sxs-lookup"><span data-stu-id="0bb77-124">overallScore</span></span>|<span data-ttu-id="0bb77-125">Int32</span><span class="sxs-lookup"><span data-stu-id="0bb77-125">Int32</span></span>|<span data-ttu-id="0bb77-126">Общий показатель категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="0bb77-126">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="0bb77-127">insights</span><span class="sxs-lookup"><span data-stu-id="0bb77-127">insights</span></span>|<span data-ttu-id="0bb77-128">Коллекция [усерекспериенцеаналитиксинсигхт](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="0bb77-128">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="0bb77-129">Аналитика для категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="0bb77-129">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="0bb77-130">state</span><span class="sxs-lookup"><span data-stu-id="0bb77-130">state</span></span>|[<span data-ttu-id="0bb77-131">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="0bb77-131">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="0bb77-132">Текущее состояние работоспособности категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="0bb77-132">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="0bb77-133">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="0bb77-133">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0bb77-134">Связи</span><span class="sxs-lookup"><span data-stu-id="0bb77-134">Relationships</span></span>
|<span data-ttu-id="0bb77-135">Связь</span><span class="sxs-lookup"><span data-stu-id="0bb77-135">Relationship</span></span>|<span data-ttu-id="0bb77-136">Тип</span><span class="sxs-lookup"><span data-stu-id="0bb77-136">Type</span></span>|<span data-ttu-id="0bb77-137">Описание</span><span class="sxs-lookup"><span data-stu-id="0bb77-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bb77-138">метриквалуес</span><span class="sxs-lookup"><span data-stu-id="0bb77-138">metricValues</span></span>|<span data-ttu-id="0bb77-139">Коллекция [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md)</span><span class="sxs-lookup"><span data-stu-id="0bb77-139">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) collection</span></span>|<span data-ttu-id="0bb77-140">Значения метрик для категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="0bb77-140">The metric values for the user experience analytics category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0bb77-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0bb77-141">JSON Representation</span></span>
<span data-ttu-id="0bb77-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0bb77-142">Here is a JSON representation of the resource.</span></span>
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
          "value": "<Unknown Primitive Type Edm.Double>"
        }
      ],
      "severity": "String"
    }
  ],
  "state": "String"
}
```



