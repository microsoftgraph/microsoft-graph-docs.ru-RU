---
title: Тип ресурса Деливерйоптимизатионбандвидсбусинесшаурслимит
description: Тип часов и процентного отношения для полосы пропускания
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ac18bb904f8992e60b6949e86439db162a3f9a36
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973815"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a><span data-ttu-id="ca585-103">Тип ресурса Деливерйоптимизатионбандвидсбусинесшаурслимит</span><span class="sxs-lookup"><span data-stu-id="ca585-103">deliveryOptimizationBandwidthBusinessHoursLimit resource type</span></span>

<span data-ttu-id="ca585-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca585-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca585-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca585-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca585-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca585-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca585-107">Тип часов и процентного отношения для полосы пропускания</span><span class="sxs-lookup"><span data-stu-id="ca585-107">Bandwidth business hours and percentages type</span></span>

## <a name="properties"></a><span data-ttu-id="ca585-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca585-108">Properties</span></span>
|<span data-ttu-id="ca585-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca585-109">Property</span></span>|<span data-ttu-id="ca585-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ca585-110">Type</span></span>|<span data-ttu-id="ca585-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ca585-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca585-112">бандвидсбегинбусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="ca585-112">bandwidthBeginBusinessHours</span></span>|<span data-ttu-id="ca585-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ca585-113">Int32</span></span>|<span data-ttu-id="ca585-114">Указывает начало рабочего времени в 24-часовом формате (0-23).</span><span class="sxs-lookup"><span data-stu-id="ca585-114">Specifies the beginning of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="ca585-115">Допустимые значения — от 0 до 23.</span><span class="sxs-lookup"><span data-stu-id="ca585-115">Valid values 0 to 23</span></span>|
|<span data-ttu-id="ca585-116">бандвидсендбусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="ca585-116">bandwidthEndBusinessHours</span></span>|<span data-ttu-id="ca585-117">Int32</span><span class="sxs-lookup"><span data-stu-id="ca585-117">Int32</span></span>|<span data-ttu-id="ca585-118">Задает время окончания рабочего дня в 24-часовом формате (0-23).</span><span class="sxs-lookup"><span data-stu-id="ca585-118">Specifies the end of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="ca585-119">Допустимые значения — от 0 до 23.</span><span class="sxs-lookup"><span data-stu-id="ca585-119">Valid values 0 to 23</span></span>|
|<span data-ttu-id="ca585-120">бандвидсперцентажедурингбусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="ca585-120">bandwidthPercentageDuringBusinessHours</span></span>|<span data-ttu-id="ca585-121">Int32</span><span class="sxs-lookup"><span data-stu-id="ca585-121">Int32</span></span>|<span data-ttu-id="ca585-122">Указывает процент пропускной способности для ограничения в рабочее время (0-100).</span><span class="sxs-lookup"><span data-stu-id="ca585-122">Specifies the percentage of bandwidth to limit during business hours (0-100).</span></span> <span data-ttu-id="ca585-123">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="ca585-123">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ca585-124">бандвидсперцентажеаутсидебусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="ca585-124">bandwidthPercentageOutsideBusinessHours</span></span>|<span data-ttu-id="ca585-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ca585-125">Int32</span></span>|<span data-ttu-id="ca585-126">Указывает процент пропускной способности, ограничивающий рабочие часы (0-100).</span><span class="sxs-lookup"><span data-stu-id="ca585-126">Specifies the percentage of bandwidth to limit outsidse business hours (0-100).</span></span> <span data-ttu-id="ca585-127">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="ca585-127">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca585-128">Связи</span><span class="sxs-lookup"><span data-stu-id="ca585-128">Relationships</span></span>
<span data-ttu-id="ca585-129">Нет</span><span class="sxs-lookup"><span data-stu-id="ca585-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca585-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca585-130">JSON Representation</span></span>
<span data-ttu-id="ca585-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca585-131">Here is a JSON representation of the resource.</span></span>
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






