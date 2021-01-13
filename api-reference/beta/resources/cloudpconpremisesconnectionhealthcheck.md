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
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a>Тип ресурса cloudPcOnPremisesConnectionHealthCheck

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Результат проверки состояния локального подключения на облачном компьютере.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[RunHealthChecks cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|Нет|Запустите проверки состояния [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемая имя для этого элемента проверки состояния.|
|status|cloudPcOnPremisesConnectionStatus|Состояние элемента проверки состояния. Только для чтения. Возможные значения: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.|
|startDateTime|DateTimeOffset|Время начала проверки состояния. Только для чтения.|
|endDateTime|DateTimeOffset|Время окончания элемента проверки состояния. Только для чтения.|
|errorType|cloudPcOnPremisesConnectionHealthCheckErrorType|Тип ошибки, которая произошла во время этой проверки. Возможные значения: `DnsCheckFqdnNotFound` , `DnsCheckUnknownError` `AdJoinCheckFqdnNotFound` `AdJoinCheckIncorrectCredentials` `AdJoinCheckOrganizationalUnitNotFound` `AdJoinCheckOrganizationalUnitIncorrectFormat` `AdJoinCheckUnknownError` `EndpointConnectivityCheckUrlNotWhitelisted` `EndpointConnectivityCheckUnknownError` `AadConnectivityCheckUnknownError` `ResourceAvailabilityCheckNoSubnetIP` `resourceAvailabilityCheckSubscriptionDisabled` `resourceAvailabilityCheckUnknownError` `permissionCheckNoSubscriptionReaderRole` `permissionCheckNoResourceGroupOwnerRole` `permissionCheckNoVNetContributorRole` `permissionCheckUnknownError` `internalServerUnknownError` .|
|recommendedAction|String|Рекомендуемое действие для устранения соответствующей ошибки.|
|additionalDetails|String|Дополнительные сведения о проверке состояния или рекомендуемом действии.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
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
