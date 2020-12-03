---
title: Тип ресурса Клаудпконпремисесконнектионхеалсчекк
description: Результат проверки работоспособности локального подключения к облачному компьютеру.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 16dea9278c9471996e4a5beaf20d5f9ec5c2d5c5
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563852"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a><span data-ttu-id="f3392-103">Тип ресурса Клаудпконпремисесконнектионхеалсчекк</span><span class="sxs-lookup"><span data-stu-id="f3392-103">cloudPcOnPremisesConnectionHealthCheck resource type</span></span>

<span data-ttu-id="f3392-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3392-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3392-105">Результат проверки работоспособности локального подключения к облачному компьютеру.</span><span class="sxs-lookup"><span data-stu-id="f3392-105">The result of a cloud PC on-premises connection health check.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="f3392-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f3392-106">Methods</span></span>

|<span data-ttu-id="f3392-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f3392-107">Method</span></span>|<span data-ttu-id="f3392-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="f3392-108">Return type</span></span>|<span data-ttu-id="f3392-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f3392-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f3392-110">Рунхеалсчеккс из Клаудпконпремисесконнектион</span><span class="sxs-lookup"><span data-stu-id="f3392-110">RunHealthChecks of cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-runhealthcheck.md)|<span data-ttu-id="f3392-111">Нет</span><span class="sxs-lookup"><span data-stu-id="f3392-111">None</span></span>|<span data-ttu-id="f3392-112">Выполнение проверок работоспособности [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="f3392-112">Run the health checks of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="f3392-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3392-113">Properties</span></span>

|<span data-ttu-id="f3392-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3392-114">Property</span></span>|<span data-ttu-id="f3392-115">Тип</span><span class="sxs-lookup"><span data-stu-id="f3392-115">Type</span></span>|<span data-ttu-id="f3392-116">Описание</span><span class="sxs-lookup"><span data-stu-id="f3392-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3392-117">displayName</span><span class="sxs-lookup"><span data-stu-id="f3392-117">displayName</span></span>|<span data-ttu-id="f3392-118">String</span><span class="sxs-lookup"><span data-stu-id="f3392-118">String</span></span>|<span data-ttu-id="f3392-119">Отображаемое имя для данного элемента проверки работоспособности.</span><span class="sxs-lookup"><span data-stu-id="f3392-119">The display name for this health check item.</span></span>|
|<span data-ttu-id="f3392-120">status</span><span class="sxs-lookup"><span data-stu-id="f3392-120">status</span></span>|<span data-ttu-id="f3392-121">клаудпконпремисесконнектионстатус</span><span class="sxs-lookup"><span data-stu-id="f3392-121">cloudPcOnPremisesConnectionStatus</span></span>|<span data-ttu-id="f3392-122">Состояние элемента "Проверка работоспособности".</span><span class="sxs-lookup"><span data-stu-id="f3392-122">The status of the health check item.</span></span> <span data-ttu-id="f3392-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3392-123">Read-only.</span></span> <span data-ttu-id="f3392-124">Возможные значения: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f3392-124">Possible values are: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.</span></span>|
|<span data-ttu-id="f3392-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f3392-125">startDateTime</span></span>|<span data-ttu-id="f3392-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3392-126">DateTimeOffset</span></span>|<span data-ttu-id="f3392-127">Время начала элемента проверки работоспособности.</span><span class="sxs-lookup"><span data-stu-id="f3392-127">The start time of the health check item.</span></span> <span data-ttu-id="f3392-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3392-128">Read-only.</span></span>|
|<span data-ttu-id="f3392-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f3392-129">endDateTime</span></span>|<span data-ttu-id="f3392-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3392-130">DateTimeOffset</span></span>|<span data-ttu-id="f3392-131">Время окончания элемента проверки работоспособности.</span><span class="sxs-lookup"><span data-stu-id="f3392-131">The end time of the health check item.</span></span> <span data-ttu-id="f3392-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3392-132">Read-only.</span></span>|
|<span data-ttu-id="f3392-133">errorType</span><span class="sxs-lookup"><span data-stu-id="f3392-133">errorType</span></span>|<span data-ttu-id="f3392-134">клаудпконпремисесконнектионхеалсчеккеррортипе</span><span class="sxs-lookup"><span data-stu-id="f3392-134">cloudPcOnPremisesConnectionHealthCheckErrorType</span></span>|<span data-ttu-id="f3392-135">Тип ошибки, возникшей во время этой проверки работоспособности.</span><span class="sxs-lookup"><span data-stu-id="f3392-135">The type of error that occurred during this health check.</span></span> <span data-ttu-id="f3392-136">Возможные значения: `DnsCheckFqdnNotFound`, `DnsCheckUnknownError`, `AdJoinCheckFqdnNotFound`, `AdJoinCheckIncorrectCredentials`, `AdJoinCheckOrganizationalUnitNotFound`, `AdJoinCheckOrganizationalUnitIncorrectFormat`, `AdJoinCheckUnknownError`, `EndpointConnectivityCheckUrlNotWhitelisted`, `EndpointConnectivityCheckUnknownError`, `AadConnectivityCheckUnknownError`.</span><span class="sxs-lookup"><span data-stu-id="f3392-136">Possible values are: `DnsCheckFqdnNotFound`, `DnsCheckUnknownError`, `AdJoinCheckFqdnNotFound`, `AdJoinCheckIncorrectCredentials`, `AdJoinCheckOrganizationalUnitNotFound`, `AdJoinCheckOrganizationalUnitIncorrectFormat`, `AdJoinCheckUnknownError`, `EndpointConnectivityCheckUrlNotWhitelisted`, `EndpointConnectivityCheckUnknownError`, `AadConnectivityCheckUnknownError`.</span></span>|
|<span data-ttu-id="f3392-137">рекоммендедактион</span><span class="sxs-lookup"><span data-stu-id="f3392-137">recommendedAction</span></span>|<span data-ttu-id="f3392-138">String</span><span class="sxs-lookup"><span data-stu-id="f3392-138">String</span></span>|<span data-ttu-id="f3392-139">Рекомендуемое действие для исправления соответствующей ошибки.</span><span class="sxs-lookup"><span data-stu-id="f3392-139">The recommended action to fix the corresponding error.</span></span>|
|<span data-ttu-id="f3392-140">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="f3392-140">additionalDetails</span></span>|<span data-ttu-id="f3392-141">String</span><span class="sxs-lookup"><span data-stu-id="f3392-141">String</span></span>|<span data-ttu-id="f3392-142">Дополнительные сведения о проверке работоспособности или рекомендуемом действии.</span><span class="sxs-lookup"><span data-stu-id="f3392-142">Additional details about the health check or the recommended action.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3392-143">Связи</span><span class="sxs-lookup"><span data-stu-id="f3392-143">Relationships</span></span>

<span data-ttu-id="f3392-144">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f3392-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3392-145">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f3392-145">JSON representation</span></span>

<span data-ttu-id="f3392-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3392-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
  "displayName": "String",
  "status": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "errorType": "String",
  "recommendedAction": "String",
  "additionalDetails": "String"
}
```
