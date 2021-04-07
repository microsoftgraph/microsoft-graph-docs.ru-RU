---
title: тип ресурса configurationManagerActionResult
description: Результат действия ConfigurationManager
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9fbe2827194403c8295e9ef59a1089c698f14092
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611981"
---
# <a name="configurationmanageractionresult-resource-type"></a>тип ресурса configurationManagerActionResult

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Результат действия ConfigurationManager


Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actionName|String|Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).|
|actionState|[actionState](../resources/intune-devices-actionstate.md)|Состояние действия, унаследованной от [deviceActionResult](../resources/intune-devices-deviceactionresult.md). Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|startDateTime|DateTimeOffset|Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).|
|lastUpdatedDateTime|DateTimeOffset|Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).|
|actionDeliveryStatus|[configurationManagerActionDeliveryStatus](../resources/intune-devices-configurationmanageractiondeliverystatus.md)|Состояние действия, доставляемого на предварительном сервере. Возможные значения: `unknown`, `pendingDelivery`, `deliveredToConnectorService`, `failedToDeliverToConnectorService`, `deliveredToOnPremisesServer`.|
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




