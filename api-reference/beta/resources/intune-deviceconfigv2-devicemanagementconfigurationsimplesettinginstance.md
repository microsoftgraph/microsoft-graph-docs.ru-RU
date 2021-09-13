---
title: тип ресурса deviceManagementConfigurationSimpleSettingInstance
description: Простой экземпляр параметра
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 579e500b099835f006e7b12876b22c1be56a5908
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030363"
---
# <a name="devicemanagementconfigurationsimplesettinginstance-resource-type"></a>тип ресурса deviceManagementConfigurationSimpleSettingInstance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Простой экземпляр параметра


Наследует [от deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|settingDefinitionId|String|Параметр Определения Id, унаследованный от [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|
|settingInstanceTemplateReference|[deviceManagementConfigurationSettingInstanceTemplateReference](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplatereference.md)|Настройка ссылки шаблона экземпляра, унаследованной от [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|
|simpleSettingValue|[deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)|Простое значение экземпляра параметра|

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
  "settingInstanceTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
    "settingInstanceTemplateId": "String"
  },
  "simpleSettingValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValue",
    "settingValueTemplateReference": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
      "settingValueTemplateId": "String",
      "useTemplateDefault": true
    },
    "value": "String"
  }
}
```



