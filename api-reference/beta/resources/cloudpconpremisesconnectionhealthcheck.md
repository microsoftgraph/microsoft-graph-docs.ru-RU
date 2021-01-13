---
title: Тип ресурса cloudPcOnPremisesConnectionHealthCheck
description: Результат проверки состояния локального подключения на облачном компьютере.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: e79f73bbe1a493e581a35db5fec396d752ff08d1
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844608"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a><span data-ttu-id="4cea9-103">Тип ресурса cloudPcOnPremisesConnectionHealthCheck</span><span class="sxs-lookup"><span data-stu-id="4cea9-103">cloudPcOnPremisesConnectionHealthCheck resource type</span></span>

<span data-ttu-id="4cea9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cea9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cea9-105">Результат проверки состояния локального подключения на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="4cea9-105">The result of a cloud PC on-premises connection health check.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="4cea9-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4cea9-106">Methods</span></span>

|<span data-ttu-id="4cea9-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4cea9-107">Method</span></span>|<span data-ttu-id="4cea9-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="4cea9-108">Return type</span></span>|<span data-ttu-id="4cea9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4cea9-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4cea9-110">RunHealthChecks cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="4cea9-110">RunHealthChecks of cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-runhealthcheck.md)|<span data-ttu-id="4cea9-111">Нет</span><span class="sxs-lookup"><span data-stu-id="4cea9-111">None</span></span>|<span data-ttu-id="4cea9-112">Запустите проверки состояния [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="4cea9-112">Run the health checks of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="4cea9-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="4cea9-113">Properties</span></span>

|<span data-ttu-id="4cea9-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="4cea9-114">Property</span></span>|<span data-ttu-id="4cea9-115">Тип</span><span class="sxs-lookup"><span data-stu-id="4cea9-115">Type</span></span>|<span data-ttu-id="4cea9-116">Описание</span><span class="sxs-lookup"><span data-stu-id="4cea9-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cea9-117">displayName</span><span class="sxs-lookup"><span data-stu-id="4cea9-117">displayName</span></span>|<span data-ttu-id="4cea9-118">String</span><span class="sxs-lookup"><span data-stu-id="4cea9-118">String</span></span>|<span data-ttu-id="4cea9-119">Отображаемая имя для этого элемента проверки состояния.</span><span class="sxs-lookup"><span data-stu-id="4cea9-119">The display name for this health check item.</span></span>|
|<span data-ttu-id="4cea9-120">status</span><span class="sxs-lookup"><span data-stu-id="4cea9-120">status</span></span>|<span data-ttu-id="4cea9-121">cloudPcOnPremisesConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="4cea9-121">cloudPcOnPremisesConnectionStatus</span></span>|<span data-ttu-id="4cea9-122">Состояние элемента проверки состояния.</span><span class="sxs-lookup"><span data-stu-id="4cea9-122">The status of the health check item.</span></span> <span data-ttu-id="4cea9-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4cea9-123">Read-only.</span></span> <span data-ttu-id="4cea9-124">Возможные значения: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4cea9-124">Possible values are: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.</span></span>|
|<span data-ttu-id="4cea9-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4cea9-125">startDateTime</span></span>|<span data-ttu-id="4cea9-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cea9-126">DateTimeOffset</span></span>|<span data-ttu-id="4cea9-127">Время начала проверки состояния.</span><span class="sxs-lookup"><span data-stu-id="4cea9-127">The start time of the health check item.</span></span> <span data-ttu-id="4cea9-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4cea9-128">Read-only.</span></span>|
|<span data-ttu-id="4cea9-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4cea9-129">endDateTime</span></span>|<span data-ttu-id="4cea9-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cea9-130">DateTimeOffset</span></span>|<span data-ttu-id="4cea9-131">Время окончания элемента проверки состояния.</span><span class="sxs-lookup"><span data-stu-id="4cea9-131">The end time of the health check item.</span></span> <span data-ttu-id="4cea9-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4cea9-132">Read-only.</span></span>|
|<span data-ttu-id="4cea9-133">errorType</span><span class="sxs-lookup"><span data-stu-id="4cea9-133">errorType</span></span>|<span data-ttu-id="4cea9-134">cloudPcOnPremisesConnectionHealthCheckErrorType</span><span class="sxs-lookup"><span data-stu-id="4cea9-134">cloudPcOnPremisesConnectionHealthCheckErrorType</span></span>|<span data-ttu-id="4cea9-135">Тип ошибки, которая произошла во время этой проверки.</span><span class="sxs-lookup"><span data-stu-id="4cea9-135">The type of error that occurred during this health check.</span></span> <span data-ttu-id="4cea9-136">Возможные значения: `DnsCheckFqdnNotFound` , `DnsCheckUnknownError` `AdJoinCheckFqdnNotFound` `AdJoinCheckIncorrectCredentials` `AdJoinCheckOrganizationalUnitNotFound` `AdJoinCheckOrganizationalUnitIncorrectFormat` `AdJoinCheckUnknownError` `EndpointConnectivityCheckUrlNotWhitelisted` `EndpointConnectivityCheckUnknownError` `AadConnectivityCheckUnknownError` `ResourceAvailabilityCheckNoSubnetIP` `resourceAvailabilityCheckSubscriptionDisabled` `resourceAvailabilityCheckUnknownError` `permissionCheckNoSubscriptionReaderRole` `permissionCheckNoResourceGroupOwnerRole` `permissionCheckNoVNetContributorRole` `permissionCheckUnknownError` `internalServerUnknownError` .</span><span class="sxs-lookup"><span data-stu-id="4cea9-136">Possible values are: `DnsCheckFqdnNotFound`, `DnsCheckUnknownError`, `AdJoinCheckFqdnNotFound`, `AdJoinCheckIncorrectCredentials`, `AdJoinCheckOrganizationalUnitNotFound`, `AdJoinCheckOrganizationalUnitIncorrectFormat`, `AdJoinCheckUnknownError`, `EndpointConnectivityCheckUrlNotWhitelisted`, `EndpointConnectivityCheckUnknownError`, `AadConnectivityCheckUnknownError`, `ResourceAvailabilityCheckNoSubnetIP`, `resourceAvailabilityCheckSubscriptionDisabled`, `resourceAvailabilityCheckUnknownError`,`permissionCheckNoSubscriptionReaderRole`, `permissionCheckNoResourceGroupOwnerRole`, `permissionCheckNoVNetContributorRole`, `permissionCheckUnknownError`, `internalServerUnknownError`.</span></span>|
|<span data-ttu-id="4cea9-137">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="4cea9-137">recommendedAction</span></span>|<span data-ttu-id="4cea9-138">String</span><span class="sxs-lookup"><span data-stu-id="4cea9-138">String</span></span>|<span data-ttu-id="4cea9-139">Рекомендуемое действие для устранения соответствующей ошибки.</span><span class="sxs-lookup"><span data-stu-id="4cea9-139">The recommended action to fix the corresponding error.</span></span>|
|<span data-ttu-id="4cea9-140">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="4cea9-140">additionalDetails</span></span>|<span data-ttu-id="4cea9-141">String</span><span class="sxs-lookup"><span data-stu-id="4cea9-141">String</span></span>|<span data-ttu-id="4cea9-142">Дополнительные сведения о проверке состояния или рекомендуемом действии.</span><span class="sxs-lookup"><span data-stu-id="4cea9-142">Additional details about the health check or the recommended action.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cea9-143">Связи</span><span class="sxs-lookup"><span data-stu-id="4cea9-143">Relationships</span></span>

<span data-ttu-id="4cea9-144">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4cea9-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4cea9-145">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4cea9-145">JSON representation</span></span>

<span data-ttu-id="4cea9-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4cea9-146">The following is a JSON representation of the resource.</span></span>
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
