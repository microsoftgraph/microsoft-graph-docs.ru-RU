---
title: Тип ресурса Клаудпконпремисесконнектионстатусдетаилс
description: Сведения о состоянии локального подключения к облачному компьютеру.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: db40df3bcd89ac21eb50870e82fe6a34ced86828
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563774"
---
# <a name="cloudpconpremisesconnectionstatusdetails-resource-type"></a><span data-ttu-id="c74d0-103">Тип ресурса Клаудпконпремисесконнектионстатусдетаилс</span><span class="sxs-lookup"><span data-stu-id="c74d0-103">cloudPcOnPremisesConnectionStatusDetails resource type</span></span>

<span data-ttu-id="c74d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c74d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c74d0-105">Сведения о состоянии [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="c74d0-105">The status details of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="c74d0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c74d0-106">Properties</span></span>

|<span data-ttu-id="c74d0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c74d0-107">Property</span></span>|<span data-ttu-id="c74d0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c74d0-108">Type</span></span>|<span data-ttu-id="c74d0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c74d0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c74d0-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c74d0-110">startDateTime</span></span>|<span data-ttu-id="c74d0-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c74d0-111">DateTimeOffset</span></span>|<span data-ttu-id="c74d0-112">Время начала проверки работоспособности подключения.</span><span class="sxs-lookup"><span data-stu-id="c74d0-112">The start time of the connection health check.</span></span> <span data-ttu-id="c74d0-113">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c74d0-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c74d0-114">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="c74d0-114">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="c74d0-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c74d0-115">endDateTime</span></span>|<span data-ttu-id="c74d0-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c74d0-116">DateTimeOffset</span></span>|<span data-ttu-id="c74d0-117">Время окончания проверки работоспособности подключения.</span><span class="sxs-lookup"><span data-stu-id="c74d0-117">The end time of the connection health check.</span></span> <span data-ttu-id="c74d0-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c74d0-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c74d0-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="c74d0-119">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="c74d0-120">хеалсчеккс</span><span class="sxs-lookup"><span data-stu-id="c74d0-120">healthChecks</span></span>|<span data-ttu-id="c74d0-121">Коллекция [клаудпконпремисесконнектионхеалсчекк](../resources/cloudpconpremisesconnectionhealthcheck.md)</span><span class="sxs-lookup"><span data-stu-id="c74d0-121">[cloudPcOnPremisesConnectionHealthCheck](../resources/cloudpconpremisesconnectionhealthcheck.md) collection</span></span>|<span data-ttu-id="c74d0-122">Все проверки, выполняемые для подключения.</span><span class="sxs-lookup"><span data-stu-id="c74d0-122">All checks that are done on the connection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c74d0-123">Связи</span><span class="sxs-lookup"><span data-stu-id="c74d0-123">Relationships</span></span>

<span data-ttu-id="c74d0-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c74d0-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c74d0-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c74d0-125">JSON representation</span></span>

<span data-ttu-id="c74d0-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c74d0-126">The following is a JSON representation of the resource.</span></span>
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
