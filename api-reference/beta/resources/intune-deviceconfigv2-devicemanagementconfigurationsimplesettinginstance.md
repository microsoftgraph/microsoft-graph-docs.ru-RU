---
title: Тип ресурса Девицеманажементконфигуратионсимплесеттингинстанце
description: Экземпляр простого параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 52ee180adbdd19ac95aa70159f198797d75ec302
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242392"
---
# <a name="devicemanagementconfigurationsimplesettinginstance-resource-type"></a>Тип ресурса Девицеманажементконфигуратионсимплесеттингинстанце

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Экземпляр простого параметра


Наследуется от [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|сеттингдефинитионид|String|Параметр ID определения, наследуемый от [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|
|симплесеттингвалуе|[девицеманажементконфигуратионсимплесеттингвалуе](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)|Значение экземпляра простого параметра|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingInstance",
  "settingDefinitionId": "String",
  "simpleSettingValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValue",
    "value": "String"
  }
}
```




