---
title: Тип ресурса Клаудпконпремисесконнектионстатусдетаилс
description: Сведения о состоянии локального подключения к облачному компьютеру.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 19dedd3344d5ed049a5b6ff5361ed7a8e4937146
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378461"
---
# <a name="cloudpconpremisesconnectionstatusdetails-resource-type"></a><span data-ttu-id="6b850-103">Тип ресурса Клаудпконпремисесконнектионстатусдетаилс</span><span class="sxs-lookup"><span data-stu-id="6b850-103">cloudPcOnPremisesConnectionStatusDetails resource type</span></span>

<span data-ttu-id="6b850-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b850-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b850-105">Сведения о состоянии [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="6b850-105">The status details of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6b850-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b850-106">Properties</span></span>

|<span data-ttu-id="6b850-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b850-107">Property</span></span>|<span data-ttu-id="6b850-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6b850-108">Type</span></span>|<span data-ttu-id="6b850-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6b850-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b850-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6b850-110">startDateTime</span></span>|<span data-ttu-id="6b850-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b850-111">DateTimeOffset</span></span>|<span data-ttu-id="6b850-112">Время начала проверки работоспособности подключения.</span><span class="sxs-lookup"><span data-stu-id="6b850-112">The start time of the connection health check.</span></span> <span data-ttu-id="6b850-113">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6b850-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6b850-114">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="6b850-114">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="6b850-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6b850-115">endDateTime</span></span>|<span data-ttu-id="6b850-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b850-116">DateTimeOffset</span></span>|<span data-ttu-id="6b850-117">Время окончания проверки работоспособности подключения.</span><span class="sxs-lookup"><span data-stu-id="6b850-117">The end time of the connection health check.</span></span> <span data-ttu-id="6b850-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6b850-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6b850-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="6b850-119">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="6b850-120">хеалсчеккс</span><span class="sxs-lookup"><span data-stu-id="6b850-120">healthChecks</span></span>|<span data-ttu-id="6b850-121">Коллекция [клаудпконпремисесконнектионхеалсчекк](../resources/cloudpconpremisesconnectionhealthcheck.md)</span><span class="sxs-lookup"><span data-stu-id="6b850-121">[cloudPcOnPremisesConnectionHealthCheck](../resources/cloudpconpremisesconnectionhealthcheck.md) collection</span></span>|<span data-ttu-id="6b850-122">Все проверки, выполняемые для подключения.</span><span class="sxs-lookup"><span data-stu-id="6b850-122">All checks that are done on the connection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b850-123">Связи</span><span class="sxs-lookup"><span data-stu-id="6b850-123">Relationships</span></span>

<span data-ttu-id="6b850-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6b850-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b850-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6b850-125">JSON representation</span></span>

<span data-ttu-id="6b850-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b850-126">The following is a JSON representation of the resource.</span></span>
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
