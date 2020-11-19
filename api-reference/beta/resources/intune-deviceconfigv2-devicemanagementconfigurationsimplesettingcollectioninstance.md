---
title: Тип ресурса Девицеманажементконфигуратионсимплесеттингколлектионинстанце
description: Экземпляр коллекции "простой параметр"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b0886b7665f1f3ce16780f2ecccc77635fd70cf3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242360"
---
# <a name="devicemanagementconfigurationsimplesettingcollectioninstance-resource-type"></a>Тип ресурса Девицеманажементконфигуратионсимплесеттингколлектионинстанце

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Экземпляр коллекции "простой параметр"


Наследуется от [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|сеттингдефинитионид|String|Параметр ID определения, наследуемый от [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|
|симплесеттингколлектионвалуе|Коллекция [девицеманажементконфигуратионсимплесеттингвалуе](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)|Значение экземпляра коллекции "Простая настройка"|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstance",
  "settingDefinitionId": "String",
  "simpleSettingCollectionValue": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValue",
      "value": "String"
    }
  ]
}
```




