---
title: тип ресурса deviceManagementConfigurationGroupSettingInstanceTemplate
description: Шаблон экземпляра настройки группы
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 260bbb9a352fd2ffc746250d749d8e2d9d044618
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58818542"
---
# <a name="devicemanagementconfigurationgroupsettinginstancetemplate-resource-type"></a>тип ресурса deviceManagementConfigurationGroupSettingInstanceTemplate

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Шаблон экземпляра настройки группы


Наследует [от deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|settingInstanceTemplateId|String|Настройка кода шаблона экземпляра, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|settingDefinitionId|String|Параметр Определения Id, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|isRequired|Boolean|Указывает, должна ли политика указать этот параметр. Унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|groupSettingValueTemplate|[deviceManagementConfigurationGroupSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationgroupsettingvaluetemplate.md)|Шаблон значения параметра группы|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationGroupSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "groupSettingValueTemplate": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValueTemplate",
    "children": [
      {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
        "settingInstanceTemplateId": "String",
        "settingDefinitionId": "String",
        "isRequired": true,
        "simpleSettingValueTemplate": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
          "settingValueTemplateId": "String",
          "defaultValue": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
            "constantValue": "String"
          }
        }
      }
    ],
    "settingValueTemplateId": "String"
  }
}
```



