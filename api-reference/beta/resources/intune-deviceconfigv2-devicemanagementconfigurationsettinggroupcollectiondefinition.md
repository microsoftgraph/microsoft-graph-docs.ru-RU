---
title: Тип ресурса deviceManagementConfigurationSettingGroupCollectionDefinition
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 238021b2c7837405419b4cf07fc112084fa940dd
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157654"
---
# <a name="devicemanagementconfigurationsettinggroupcollectiondefinition-resource-type"></a>Тип ресурса deviceManagementConfigurationSettingGroupCollectionDefinition

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.


Наследуется [от deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementConfigurationSettingGroupCollectionDefinitions](../api/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition-list.md)|[Коллекция deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)|Список свойств и связей объектов [deviceManagementConfigurationSettingGroupCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)|
|[Get deviceManagementConfigurationSettingGroupCollectionDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition-get.md)|[deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)|Чтение свойств и связей объекта [deviceManagementConfigurationSettingGroupCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)|
|[Создание deviceManagementConfigurationSettingGroupCollectionDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition-create.md)|[deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)|Создание объекта [deviceManagementConfigurationSettingGroupCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)|
|[Удаление deviceManagementConfigurationSettingGroupCollectionDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition-delete.md)|Нет|Удаляет [deviceManagementConfigurationSettingGroupCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)|
|[Обновление deviceManagementConfigurationSettingGroupCollectionDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition-update.md)|[deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)|Обновление свойств объекта [deviceManagementConfigurationSettingGroupCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|применимость|[deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|Сведения о том, какой параметр устройства применим к inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|accessTypes|[deviceManagementConfigurationSettingAccessTypes](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|Режим доступа для чтения и записи параметра. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.|
|keywords|Коллекция String|Маркеры для поиска параметров на унаследованных от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|infoUrls|Коллекция String|Список ссылок, дополнительные сведения о параметре можно найти по адресу Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|occurrence|[deviceManagementConfigurationSettingOccurrence](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|Указывает, требуется ли параметр или не наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|baseUri|String|Базовый путь CSP Наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|offsetUri|String|Смещение пути CSP от Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|rootDefinitionId|String|Определение корневого параметра, если этот параметр является параметром-дитя. Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|categoryId|String|Указывает группу области, в которой настроен параметр в указанном поставщике служб конфигурации (CSP), наследуемом от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|settingUsage|[deviceManagementConfigurationSettingUsage](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|Тип параметра, например конфигурация и соответствие. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) Возможные значения: `none`, `configuration`.|
|uxBehavior|[deviceManagementConfigurationControlType](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|Представление типа параметра в UX. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.|
|id|String|Идентификатор элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|description|String|Описание элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|helpText|String|Текст справки для элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|name|String|Имя элемента. Наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|displayName|String|Отображающее имя элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|version|String|Версия элемента. Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|childIds|Коллекция String|Зависимые параметры для этой группы параметров. Наследуется от [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)|
|dependentOn|[Коллекция deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)|Список зависимостей для группы параметров Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)|
|dependedOnBy|[Коллекция deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)|Список параметров, которые зависят от этого параметра. Наследуется от [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)|
|maximumCount|Int32|Максимальное количество параметров в коллекции. Допустимые значения: от 1 до 100|
|minimumCount|Int32|Минимальное количество параметров в коллекции. Допустимые значения: от 1 до 100|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingGroupCollectionDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupCollectionDefinition",
  "applicability": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
    "description": "String",
    "platform": "String",
    "deviceMode": "String",
    "technologies": "String"
  },
  "accessTypes": "String",
  "keywords": [
    "String"
  ],
  "infoUrls": [
    "String"
  ],
  "occurrence": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
    "minDeviceOccurrence": 1024,
    "maxDeviceOccurrence": 1024
  },
  "baseUri": "String",
  "offsetUri": "String",
  "rootDefinitionId": "String",
  "categoryId": "String",
  "settingUsage": "String",
  "uxBehavior": "String",
  "id": "String (identifier)",
  "description": "String",
  "helpText": "String",
  "name": "String",
  "displayName": "String",
  "version": "String",
  "childIds": [
    "String"
  ],
  "dependentOn": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn",
      "dependentOn": "String",
      "parentSettingId": "String"
    }
  ],
  "dependedOnBy": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
      "dependedOnBy": "String",
      "required": true
    }
  ],
  "maximumCount": 1024,
  "minimumCount": 1024
}
```




