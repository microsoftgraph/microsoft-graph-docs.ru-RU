---
title: тип ресурса deviceManagementConfigurationGroupSettingValueTemplate
description: Шаблон значения параметра группы
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ecb0efaedac1cc507565ab41b92be23bb88d4edc
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58818528"
---
# <a name="devicemanagementconfigurationgroupsettingvaluetemplate-resource-type"></a>тип ресурса deviceManagementConfigurationGroupSettingValueTemplate

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Шаблон значения параметра группы

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|children|[коллекция deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|Дети параметров группы|
|settingValueTemplateId|String|Настройка кода шаблона значений|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValueTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationGroupSettingValueTemplate",
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
```



