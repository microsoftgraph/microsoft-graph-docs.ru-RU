---
title: тип ресурса cloudPcOnPremisesConnectionStatusDetails
description: Сведения о состоянии локального подключения облачного КОМПЬЮТЕРА.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 7ef9847190fb851482d29535d0709f3d74bbf3aa
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722180"
---
# <a name="cloudpconpremisesconnectionstatusdetails-resource-type"></a><span data-ttu-id="da8d5-103">тип ресурса cloudPcOnPremisesConnectionStatusDetails</span><span class="sxs-lookup"><span data-stu-id="da8d5-103">cloudPcOnPremisesConnectionStatusDetails resource type</span></span>

<span data-ttu-id="da8d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da8d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da8d5-105">Сведения о состоянии [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="da8d5-105">The status details of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="da8d5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="da8d5-106">Properties</span></span>

|<span data-ttu-id="da8d5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="da8d5-107">Property</span></span>|<span data-ttu-id="da8d5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="da8d5-108">Type</span></span>|<span data-ttu-id="da8d5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="da8d5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da8d5-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="da8d5-110">startDateTime</span></span>|<span data-ttu-id="da8d5-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da8d5-111">DateTimeOffset</span></span>|<span data-ttu-id="da8d5-112">Время начала проверки состояния подключения.</span><span class="sxs-lookup"><span data-stu-id="da8d5-112">The start time of the connection health check.</span></span> <span data-ttu-id="da8d5-113">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="da8d5-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="da8d5-114">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="da8d5-114">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="da8d5-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="da8d5-115">endDateTime</span></span>|<span data-ttu-id="da8d5-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da8d5-116">DateTimeOffset</span></span>|<span data-ttu-id="da8d5-117">Конечное время проверки состояния подключения.</span><span class="sxs-lookup"><span data-stu-id="da8d5-117">The end time of the connection health check.</span></span> <span data-ttu-id="da8d5-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="da8d5-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="da8d5-119">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="da8d5-119">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="da8d5-120">healthChecks</span><span class="sxs-lookup"><span data-stu-id="da8d5-120">healthChecks</span></span>|<span data-ttu-id="da8d5-121">[коллекция cloudPcOnPremisesConnectionHealthCheck](../resources/cloudpconpremisesconnectionhealthcheck.md)</span><span class="sxs-lookup"><span data-stu-id="da8d5-121">[cloudPcOnPremisesConnectionHealthCheck](../resources/cloudpconpremisesconnectionhealthcheck.md) collection</span></span>|<span data-ttu-id="da8d5-122">Все проверки, которые проводятся в подключении.</span><span class="sxs-lookup"><span data-stu-id="da8d5-122">All checks that are done on the connection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da8d5-123">Связи</span><span class="sxs-lookup"><span data-stu-id="da8d5-123">Relationships</span></span>

<span data-ttu-id="da8d5-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="da8d5-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="da8d5-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="da8d5-125">JSON representation</span></span>

<span data-ttu-id="da8d5-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da8d5-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionStatusDetails"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnectionStatusDetails",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "healthChecks": [
    {
      "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
      "displayName": "String",
      "status": "String",
      "startDateTime": "String (timestamp)",
      "endDateTime": "String (timestamp)",
      "errorType": "String",
      "recommendedAction": "String",
      "additionalDetails": "String"
    }
  ]
}
```
