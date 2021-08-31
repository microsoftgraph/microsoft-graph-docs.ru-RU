---
title: тип ресурса deviceManagementConfigurationChoiceSettingInstanceTemplate
description: Шаблон параметра выбор экземпляра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f8448978899a254b66d2494eb09e9fa8b08b8293
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786651"
---
# <a name="devicemanagementconfigurationchoicesettinginstancetemplate-resource-type"></a>тип ресурса deviceManagementConfigurationChoiceSettingInstanceTemplate

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Шаблон параметра выбор экземпляра


Наследует [от deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|settingInstanceTemplateId|Строка|Настройка кода шаблона экземпляра, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|settingDefinitionId|Строка|Параметр Определения Id, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|isRequired|Boolean|Указывает, должна ли политика указать этот параметр. Унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|choiceSettingValueTemplate|[deviceManagementConfigurationChoiceSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluetemplate.md)|Шаблон параметра параметра выбор|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "choiceSettingValueTemplate": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueTemplate",
    "defaultValue": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate",
      "settingDefinitionOptionId": "String",
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
      ]
    },
    "recommendedValueDefinition": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
      "allowedOptions": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
          "itemId": "String",
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
          ]
        }
      ]
    },
    "requiredValueDefinition": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
      "allowedOptions": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
          "itemId": "String",
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
          ]
        }
      ]
    },
    "settingValueTemplateId": "String"
  }
}
```



