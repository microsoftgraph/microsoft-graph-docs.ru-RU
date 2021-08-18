---
title: тип ресурса deviceManagementConfigurationChoiceSettingValueTemplate
description: Шаблон параметра параметра выбор
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d934f6c8c4e00f6254e20b255b9935e0fff5004d91279b00dd947ef0e3af9c9d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54153057"
---
# <a name="devicemanagementconfigurationchoicesettingvaluetemplate-resource-type"></a>тип ресурса deviceManagementConfigurationChoiceSettingValueTemplate

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Шаблон параметра параметра выбор

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|defaultValue|[deviceManagementConfigurationChoiceSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefaulttemplate.md)|Шаблон параметра параметра значение по умолчанию.|
|recommendedValueDefinition|[deviceManagementConfigurationChoiceSettingValueDefinitionTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefinitiontemplate.md)|Рекомендуемые переопределения определения.|
|requiredValueDefinition|[deviceManagementConfigurationChoiceSettingValueDefinitionTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefinitiontemplate.md)|Обязательное переопределения определения.|
|settingValueTemplateId|String|Настройка кода шаблона значений|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingValueTemplate",
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
```




