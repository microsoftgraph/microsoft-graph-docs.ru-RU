---
title: Тип ресурса Конфигуратионманажерактионресулт
description: Результат действия Конфигуратионманажер
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6c73775293385ecfcef8ef269a2f3e83c53b233f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691409"
---
# <a name="configurationmanageractionresult-resource-type"></a>Тип ресурса Конфигуратионманажерактионресулт

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Результат действия Конфигуратионманажер


Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actionName|String|Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md). Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|startDateTime|DateTimeOffset|Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).|
|lastUpdatedDateTime|DateTimeOffset|Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).|
|актионделиверистатус|[configurationManagerActionDeliveryStatus](../resources/intune-devices-configurationmanageractiondeliverystatus.md)|Состояние действия, которое доставляется на локальный сервер. Возможные значения: `unknown`, `pendingDelivery`, `deliveredToConnectorService`, `failedToDeliverToConnectorService`, `deliveredToOnPremisesServer`.|
|errorCode|Int32|Код ошибки действия Configuration Manager от клиента|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "actionDeliveryStatus": "String",
  "errorCode": 1024
}
```





