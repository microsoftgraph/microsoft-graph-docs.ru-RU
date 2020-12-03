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
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a>Тип ресурса Клаудпконпремисесконнектионхеалсчекк

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Результат проверки работоспособности локального подключения к облачному компьютеру.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Рунхеалсчеккс из Клаудпконпремисесконнектион](../api/cloudpconpremisesconnection-runhealthcheck.md)|Нет|Выполнение проверок работоспособности [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md).|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя для данного элемента проверки работоспособности.|
|status|клаудпконпремисесконнектионстатус|Состояние элемента "Проверка работоспособности". Только для чтения. Возможные значения: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.|
|startDateTime|DateTimeOffset|Время начала элемента проверки работоспособности. Только для чтения.|
|endDateTime|DateTimeOffset|Время окончания элемента проверки работоспособности. Только для чтения.|
|errorType|клаудпконпремисесконнектионхеалсчеккеррортипе|Тип ошибки, возникшей во время этой проверки работоспособности. Возможные значения: `DnsCheckFqdnNotFound`, `DnsCheckUnknownError`, `AdJoinCheckFqdnNotFound`, `AdJoinCheckIncorrectCredentials`, `AdJoinCheckOrganizationalUnitNotFound`, `AdJoinCheckOrganizationalUnitIncorrectFormat`, `AdJoinCheckUnknownError`, `EndpointConnectivityCheckUrlNotWhitelisted`, `EndpointConnectivityCheckUnknownError`, `AadConnectivityCheckUnknownError`.|
|рекоммендедактион|String|Рекомендуемое действие для исправления соответствующей ошибки.|
|additionalDetails|String|Дополнительные сведения о проверке работоспособности или рекомендуемом действии.|

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
