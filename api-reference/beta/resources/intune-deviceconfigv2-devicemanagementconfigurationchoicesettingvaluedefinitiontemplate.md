---
title: deviceManagementConfigurationChoiceSettingValueDefinitionTemplate type
description: Шаблон определения значения параметра выбор
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3dfb38c67777344f5489c4593d89dcd140370abf0d77e5a874ae50656ef6f35
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54193729"
---
# <a name="devicemanagementconfigurationchoicesettingvaluedefinitiontemplate-resource-type"></a>deviceManagementConfigurationChoiceSettingValueDefinitionTemplate type

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Шаблон определения значения параметра выбор

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedOptions|[коллекция deviceManagementConfigurationOptionDefinitionTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinitiontemplate.md)|Допустимые параметры параметра выбора|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
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
}
```




