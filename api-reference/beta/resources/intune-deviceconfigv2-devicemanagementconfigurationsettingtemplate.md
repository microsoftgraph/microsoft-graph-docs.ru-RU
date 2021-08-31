---
title: тип ресурса deviceManagementConfigurationSettingTemplate
description: Шаблон параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 78499c007ae2e2e7659fe49bd91ada31e6230197
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58804283"
---
# <a name="devicemanagementconfigurationsettingtemplate-resource-type"></a>тип ресурса deviceManagementConfigurationSettingTemplate

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Шаблон параметра

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementConfigurationSettingTemplates](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate-list.md)|[коллекция deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|Список свойств и связей [объектов deviceManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|
|[Get deviceManagementConfigurationSettingTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate-get.md)|[deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|Чтение свойств и связей [объекта deviceManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|
|[Создание deviceManagementConfigurationSettingTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate-create.md)|[deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|Создайте новый [объект deviceManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|
|[Удаление deviceManagementConfigurationSettingTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate-delete.md)|Нет|Удаляет [устройствоManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|
|[Обновление deviceManagementConfigurationSettingTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate-update.md)|[deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|Обновление свойств объекта [deviceManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ этого шаблона параметра в шаблоне политики, который содержит его. Автоматически созданный.|
|settingInstanceTemplate|[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|Настройка шаблона экземпляра|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|settingDefinitions|[коллекция deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|Список связанных определений параметров|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingTemplate",
  "id": "String (identifier)",
  "settingInstanceTemplate": {
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
}
```



