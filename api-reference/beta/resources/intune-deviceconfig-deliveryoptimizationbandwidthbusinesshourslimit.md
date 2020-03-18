---
title: Тип ресурса Деливерйоптимизатионбандвидсбусинесшаурслимит
description: Тип часов и процентного отношения для полосы пропускания
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 83e0402e7b63925e8c02c87a5c1abd9b08c9c8c6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794391"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a><span data-ttu-id="3ef33-103">Тип ресурса Деливерйоптимизатионбандвидсбусинесшаурслимит</span><span class="sxs-lookup"><span data-stu-id="3ef33-103">deliveryOptimizationBandwidthBusinessHoursLimit resource type</span></span>

> <span data-ttu-id="3ef33-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ef33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ef33-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ef33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ef33-106">Тип часов и процентного отношения для полосы пропускания</span><span class="sxs-lookup"><span data-stu-id="3ef33-106">Bandwidth business hours and percentages type</span></span>

## <a name="properties"></a><span data-ttu-id="3ef33-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ef33-107">Properties</span></span>
|<span data-ttu-id="3ef33-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ef33-108">Property</span></span>|<span data-ttu-id="3ef33-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3ef33-109">Type</span></span>|<span data-ttu-id="3ef33-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3ef33-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ef33-111">бандвидсбегинбусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="3ef33-111">bandwidthBeginBusinessHours</span></span>|<span data-ttu-id="3ef33-112">Int32</span><span class="sxs-lookup"><span data-stu-id="3ef33-112">Int32</span></span>|<span data-ttu-id="3ef33-113">Указывает начало рабочего времени в 24-часовом формате (0-23).</span><span class="sxs-lookup"><span data-stu-id="3ef33-113">Specifies the beginning of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="3ef33-114">Допустимые значения — от 0 до 23.</span><span class="sxs-lookup"><span data-stu-id="3ef33-114">Valid values 0 to 23</span></span>|
|<span data-ttu-id="3ef33-115">бандвидсендбусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="3ef33-115">bandwidthEndBusinessHours</span></span>|<span data-ttu-id="3ef33-116">Int32</span><span class="sxs-lookup"><span data-stu-id="3ef33-116">Int32</span></span>|<span data-ttu-id="3ef33-117">Задает время окончания рабочего дня в 24-часовом формате (0-23).</span><span class="sxs-lookup"><span data-stu-id="3ef33-117">Specifies the end of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="3ef33-118">Допустимые значения — от 0 до 23.</span><span class="sxs-lookup"><span data-stu-id="3ef33-118">Valid values 0 to 23</span></span>|
|<span data-ttu-id="3ef33-119">бандвидсперцентажедурингбусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="3ef33-119">bandwidthPercentageDuringBusinessHours</span></span>|<span data-ttu-id="3ef33-120">Int32</span><span class="sxs-lookup"><span data-stu-id="3ef33-120">Int32</span></span>|<span data-ttu-id="3ef33-121">Указывает процент пропускной способности для ограничения в рабочее время (0-100).</span><span class="sxs-lookup"><span data-stu-id="3ef33-121">Specifies the percentage of bandwidth to limit during business hours (0-100).</span></span> <span data-ttu-id="3ef33-122">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="3ef33-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="3ef33-123">бандвидсперцентажеаутсидебусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="3ef33-123">bandwidthPercentageOutsideBusinessHours</span></span>|<span data-ttu-id="3ef33-124">Int32</span><span class="sxs-lookup"><span data-stu-id="3ef33-124">Int32</span></span>|<span data-ttu-id="3ef33-125">Указывает процент пропускной способности, ограничивающий рабочие часы (0-100).</span><span class="sxs-lookup"><span data-stu-id="3ef33-125">Specifies the percentage of bandwidth to limit outsidse business hours (0-100).</span></span> <span data-ttu-id="3ef33-126">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="3ef33-126">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ef33-127">Связи</span><span class="sxs-lookup"><span data-stu-id="3ef33-127">Relationships</span></span>
<span data-ttu-id="3ef33-128">Нет</span><span class="sxs-lookup"><span data-stu-id="3ef33-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ef33-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ef33-129">JSON Representation</span></span>
<span data-ttu-id="3ef33-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ef33-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
  "bandwidthBeginBusinessHours": 1024,
  "bandwidthEndBusinessHours": 1024,
  "bandwidthPercentageDuringBusinessHours": 1024,
  "bandwidthPercentageOutsideBusinessHours": 1024
}
```



