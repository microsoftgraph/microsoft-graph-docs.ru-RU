---
title: deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate type
description: Шаблон экземпляра простой коллекции параметров
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bbde0eeccd0e89669a8d2d86fa2897c9d794831f42b08b4801af76ea404d7adc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54198075"
---
# <a name="devicemanagementconfigurationsimplesettingcollectioninstancetemplate-resource-type"></a>deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate type

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Шаблон экземпляра простой коллекции параметров


Наследует [от deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|settingInstanceTemplateId|Строка|Настройка кода шаблона экземпляра, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|settingDefinitionId|Строка|Параметр Определения Id, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|isRequired|Boolean|Указывает, должна ли политика указать этот параметр. Унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|simpleSettingCollectionValueTemplate|[коллекция deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)|Шаблон значения простого параметра коллекции|
|allowUnmanagedValues|Логический|Связанная политика может при добавлении значений, которые не присутствуют в шаблоне.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "simpleSettingCollectionValueTemplate": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
      "settingValueTemplateId": "String",
      "defaultValue": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
        "constantValue": "String"
      }
    }
  ],
  "allowUnmanagedValues": true
}
```




