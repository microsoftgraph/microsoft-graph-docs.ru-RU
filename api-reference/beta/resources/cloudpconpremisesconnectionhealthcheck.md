---
title: Тип ресурса Клаудпконпремисесконнектионхеалсчекк
description: Результат проверки работоспособности локального подключения к облачному компьютеру.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 188d9db2dbef3b3e731e0c95a48f6637e3e00101
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378515"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a><span data-ttu-id="70011-103">Тип ресурса Клаудпконпремисесконнектионхеалсчекк</span><span class="sxs-lookup"><span data-stu-id="70011-103">cloudPcOnPremisesConnectionHealthCheck resource type</span></span>

<span data-ttu-id="70011-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70011-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70011-105">Результат проверки работоспособности локального подключения к облачному компьютеру.</span><span class="sxs-lookup"><span data-stu-id="70011-105">The result of a cloud PC on-premises connection health check.</span></span>

## <a name="methods"></a><span data-ttu-id="70011-106">Методы</span><span class="sxs-lookup"><span data-stu-id="70011-106">Methods</span></span>

|<span data-ttu-id="70011-107">Метод</span><span class="sxs-lookup"><span data-stu-id="70011-107">Method</span></span>|<span data-ttu-id="70011-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="70011-108">Return type</span></span>|<span data-ttu-id="70011-109">Описание</span><span class="sxs-lookup"><span data-stu-id="70011-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="70011-110">Рунхеалсчеккс из Клаудпконпремисесконнектион</span><span class="sxs-lookup"><span data-stu-id="70011-110">RunHealthChecks of cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-runhealthcheck.md)|<span data-ttu-id="70011-111">Нет</span><span class="sxs-lookup"><span data-stu-id="70011-111">None</span></span>|<span data-ttu-id="70011-112">Выполнение проверок работоспособности [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="70011-112">Run the health checks of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="70011-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="70011-113">Properties</span></span>

|<span data-ttu-id="70011-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="70011-114">Property</span></span>|<span data-ttu-id="70011-115">Тип</span><span class="sxs-lookup"><span data-stu-id="70011-115">Type</span></span>|<span data-ttu-id="70011-116">Описание</span><span class="sxs-lookup"><span data-stu-id="70011-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70011-117">displayName</span><span class="sxs-lookup"><span data-stu-id="70011-117">displayName</span></span>|<span data-ttu-id="70011-118">Строка</span><span class="sxs-lookup"><span data-stu-id="70011-118">String</span></span>|<span data-ttu-id="70011-119">Отображаемое имя для данного элемента проверки работоспособности.</span><span class="sxs-lookup"><span data-stu-id="70011-119">The display name for this health check item.</span></span>|
|<span data-ttu-id="70011-120">status</span><span class="sxs-lookup"><span data-stu-id="70011-120">status</span></span>|<span data-ttu-id="70011-121">клаудпконпремисесконнектионстатус</span><span class="sxs-lookup"><span data-stu-id="70011-121">cloudPcOnPremisesConnectionStatus</span></span>|<span data-ttu-id="70011-122">Состояние элемента "Проверка работоспособности".</span><span class="sxs-lookup"><span data-stu-id="70011-122">The status of the health check item.</span></span> <span data-ttu-id="70011-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="70011-123">Read-only.</span></span> <span data-ttu-id="70011-124">Возможные значения: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="70011-124">Possible values are: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.</span></span>|
|<span data-ttu-id="70011-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="70011-125">startDateTime</span></span>|<span data-ttu-id="70011-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70011-126">DateTimeOffset</span></span>|<span data-ttu-id="70011-127">Время начала элемента проверки работоспособности.</span><span class="sxs-lookup"><span data-stu-id="70011-127">The start time of the health check item.</span></span> <span data-ttu-id="70011-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="70011-128">Read-only.</span></span>|
|<span data-ttu-id="70011-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="70011-129">endDateTime</span></span>|<span data-ttu-id="70011-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70011-130">DateTimeOffset</span></span>|<span data-ttu-id="70011-131">Время окончания элемента проверки работоспособности.</span><span class="sxs-lookup"><span data-stu-id="70011-131">The end time of the health check item.</span></span> <span data-ttu-id="70011-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="70011-132">Read-only.</span></span>|
|<span data-ttu-id="70011-133">errorType</span><span class="sxs-lookup"><span data-stu-id="70011-133">errorType</span></span>|<span data-ttu-id="70011-134">клаудпконпремисесконнектионхеалсчеккеррортипе</span><span class="sxs-lookup"><span data-stu-id="70011-134">cloudPcOnPremisesConnectionHealthCheckErrorType</span></span>|<span data-ttu-id="70011-135">Тип ошибки, возникшей во время этой проверки работоспособности.</span><span class="sxs-lookup"><span data-stu-id="70011-135">The type of error that occurred during this health check.</span></span> <span data-ttu-id="70011-136">Возможные значения: `DnsCheckFqdnNotFound`, `DnsCheckUnknownError`, `AdJoinCheckFqdnNotFound`, `AdJoinCheckIncorrectCredentials`, `AdJoinCheckOrganizationalUnitNotFound`, `AdJoinCheckOrganizationalUnitIncorrectFormat`, `AdJoinCheckUnknownError`, `EndpointConnectivityCheckUrlNotWhitelisted`, `EndpointConnectivityCheckUnknownError`, `AadConnectivityCheckUnknownError`.</span><span class="sxs-lookup"><span data-stu-id="70011-136">Possible values are: `DnsCheckFqdnNotFound`, `DnsCheckUnknownError`, `AdJoinCheckFqdnNotFound`, `AdJoinCheckIncorrectCredentials`, `AdJoinCheckOrganizationalUnitNotFound`, `AdJoinCheckOrganizationalUnitIncorrectFormat`, `AdJoinCheckUnknownError`, `EndpointConnectivityCheckUrlNotWhitelisted`, `EndpointConnectivityCheckUnknownError`, `AadConnectivityCheckUnknownError`.</span></span>|
|<span data-ttu-id="70011-137">рекоммендедактион</span><span class="sxs-lookup"><span data-stu-id="70011-137">recommendedAction</span></span>|<span data-ttu-id="70011-138">Строка</span><span class="sxs-lookup"><span data-stu-id="70011-138">String</span></span>|<span data-ttu-id="70011-139">Рекомендуемое действие для исправления соответствующей ошибки.</span><span class="sxs-lookup"><span data-stu-id="70011-139">The recommended action to fix the corresponding error.</span></span>|
|<span data-ttu-id="70011-140">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="70011-140">additionalDetails</span></span>|<span data-ttu-id="70011-141">Строка</span><span class="sxs-lookup"><span data-stu-id="70011-141">String</span></span>|<span data-ttu-id="70011-142">Дополнительные сведения о проверке работоспособности или рекомендуемом действии.</span><span class="sxs-lookup"><span data-stu-id="70011-142">Additional details about the health check or the recommended action.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70011-143">Связи</span><span class="sxs-lookup"><span data-stu-id="70011-143">Relationships</span></span>

<span data-ttu-id="70011-144">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="70011-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="70011-145">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="70011-145">JSON representation</span></span>

<span data-ttu-id="70011-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70011-146">The following is a JSON representation of the resource.</span></span>
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
