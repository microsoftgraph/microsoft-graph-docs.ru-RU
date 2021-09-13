---
title: тип ресурса deviceManagementConfigurationIntegerSettingValueTemplate
description: Шаблон параметра integer
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 05b58a5c329a190733a9b4759b83054a52479b9f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148230"
---
# <a name="devicemanagementconfigurationintegersettingvaluetemplate-resource-type"></a>тип ресурса deviceManagementConfigurationIntegerSettingValueTemplate

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Шаблон параметра integer


Наследует [от deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|settingValueTemplateId|String|Настройка кода шаблона значений, унаследованный от [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)|
|defaultValue|[deviceManagementConfigurationIntegerSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationintegersettingvaluedefaulttemplate.md)|Integer Setting Value Default Template.|
|recommendedValueDefinition|[deviceManagementConfigurationIntegerSettingValueDefinitionTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationintegersettingvaluedefinitiontemplate.md)|Рекомендуемое определение значения.|
|requiredValueDefinition|[deviceManagementConfigurationIntegerSettingValueDefinitionTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationintegersettingvaluedefinitiontemplate.md)|Обязательное определение значения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValueTemplate",
  "settingValueTemplateId": "String",
  "defaultValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate",
    "constantValue": 1024
  },
  "recommendedValueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate",
    "minValue": 1024,
    "maxValue": 1024
  },
  "requiredValueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate",
    "minValue": 1024,
    "maxValue": 1024
  }
}
```



