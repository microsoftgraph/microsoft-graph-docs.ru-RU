---
title: Тип ресурса Усерекспериенцеаналитиксинсигхт
description: Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 36277b147e7eabc6f28aef3877538ebbc429f381
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36341240"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a><span data-ttu-id="b6523-103">Тип ресурса Усерекспериенцеаналитиксинсигхт</span><span class="sxs-lookup"><span data-stu-id="b6523-103">userExperienceAnalyticsInsight resource type</span></span>

> <span data-ttu-id="b6523-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6523-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6523-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6523-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6523-106">Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="b6523-106">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="b6523-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6523-107">Properties</span></span>
|<span data-ttu-id="b6523-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6523-108">Property</span></span>|<span data-ttu-id="b6523-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b6523-109">Type</span></span>|<span data-ttu-id="b6523-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b6523-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6523-111">усерекспериенцеаналитиксметриЦид</span><span class="sxs-lookup"><span data-stu-id="b6523-111">userExperienceAnalyticsMetricId</span></span>|<span data-ttu-id="b6523-112">String</span><span class="sxs-lookup"><span data-stu-id="b6523-112">String</span></span>|<span data-ttu-id="b6523-113">Уникальный идентификатор аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="b6523-113">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="b6523-114">инсигхтид</span><span class="sxs-lookup"><span data-stu-id="b6523-114">insightId</span></span>|<span data-ttu-id="b6523-115">String</span><span class="sxs-lookup"><span data-stu-id="b6523-115">String</span></span>|<span data-ttu-id="b6523-116">Уникальный идентификатор аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="b6523-116">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="b6523-117">значение</span><span class="sxs-lookup"><span data-stu-id="b6523-117">value</span></span>|<span data-ttu-id="b6523-118">Коллекция [усерекспериенцеаналитиксинсигхтвалуе](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b6523-118">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md) collection</span></span>|<span data-ttu-id="b6523-119">Значение аналитического интерфейса пользователя.</span><span class="sxs-lookup"><span data-stu-id="b6523-119">The value of the user experience analytics insight.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6523-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="b6523-120">Relationships</span></span>
<span data-ttu-id="b6523-121">Нет</span><span class="sxs-lookup"><span data-stu-id="b6523-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6523-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6523-122">JSON Representation</span></span>
<span data-ttu-id="b6523-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6523-123">Here is a JSON representation of the resource.</span></span>
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
  "value": [
    {
      "@odata.type": "microsoft.graph.insightValueDouble"
    }
  ]
}
```



