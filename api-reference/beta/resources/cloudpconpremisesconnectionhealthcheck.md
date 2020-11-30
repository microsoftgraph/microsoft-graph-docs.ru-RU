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
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a>Тип ресурса Клаудпконпремисесконнектионхеалсчекк

Пространство имен: microsoft.graph

Результат проверки работоспособности локального подключения к облачному компьютеру.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Рунхеалсчеккс из Клаудпконпремисесконнектион](../api/cloudpconpremisesconnection-runhealthcheck.md)|Нет|Выполнение проверок работоспособности [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md).|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя для данного элемента проверки работоспособности.|
|status|клаудпконпремисесконнектионстатус|Состояние элемента "Проверка работоспособности". Только для чтения. Возможные значения: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.|
|startDateTime|DateTimeOffset|Время начала элемента проверки работоспособности. Только для чтения.|
|endDateTime|DateTimeOffset|Время окончания элемента проверки работоспособности. Только для чтения.|
|errorType|клаудпконпремисесконнектионхеалсчеккеррортипе|Тип ошибки, возникшей во время этой проверки работоспособности. Возможные значения: `DnsCheckFqdnNotFound`, `DnsCheckUnknownError`, `AdJoinCheckFqdnNotFound`, `AdJoinCheckIncorrectCredentials`, `AdJoinCheckOrganizationalUnitNotFound`, `AdJoinCheckOrganizationalUnitIncorrectFormat`, `AdJoinCheckUnknownError`, `EndpointConnectivityCheckUrlNotWhitelisted`, `EndpointConnectivityCheckUnknownError`, `AadConnectivityCheckUnknownError`.|
|рекоммендедактион|Строка|Рекомендуемое действие для исправления соответствующей ошибки.|
|additionalDetails|Строка|Дополнительные сведения о проверке работоспособности или рекомендуемом действии.|

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
