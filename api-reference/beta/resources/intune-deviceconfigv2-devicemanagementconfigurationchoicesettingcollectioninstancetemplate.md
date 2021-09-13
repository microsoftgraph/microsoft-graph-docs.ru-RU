---
title: тип ресурса deviceManagementConfigurationChoiceSettingCollectionInstanceTemplate
description: Шаблон экземпляра параметра выбор коллекции
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 601780e1d882a34b04bbb4dabc21390eda7ed0f9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129049"
---
# <a name="devicemanagementconfigurationchoicesettingcollectioninstancetemplate-resource-type"></a>тип ресурса deviceManagementConfigurationChoiceSettingCollectionInstanceTemplate

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Шаблон экземпляра параметра выбор коллекции


Наследует [от deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|settingInstanceTemplateId|String|Настройка кода шаблона экземпляра, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|settingDefinitionId|String|Параметр Определения Id, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|isRequired|Boolean|Указывает, должна ли политика указать этот параметр. Унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|choiceSettingCollectionValueTemplate|[коллекция deviceManagementConfigurationChoiceSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluetemplate.md)|Шаблон значения параметра выбор коллекции|
|allowUnmanagedValues|Логическое|Связанная политика может при добавлении значений, которые не присутствуют в шаблоне.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "choiceSettingCollectionValueTemplate": [
    {
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
  ],
  "allowUnmanagedValues": true
}
```



