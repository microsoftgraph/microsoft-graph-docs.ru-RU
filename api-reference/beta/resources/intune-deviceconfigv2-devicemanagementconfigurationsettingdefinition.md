---
title: Тип ресурса deviceManagementConfigurationSettingDefinition
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 206b243c45936efa289024d26051edacc41a2171
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66667875"
---
# <a name="devicemanagementconfigurationsettingdefinition-resource-type"></a>Тип ресурса deviceManagementConfigurationSettingDefinition

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов deviceManagementConfigurationSettingDefinitions](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition-list.md)|[Коллекция deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|Список свойств и связей объектов [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) .|
|[Получение объекта deviceManagementConfigurationSettingDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition-get.md)|[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|Чтение свойств и связей объекта [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) .|
|[Создание объекта deviceManagementConfigurationSettingDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition-create.md)|[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|Создайте объект [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) .|
|[Удаление объекта deviceManagementConfigurationSettingDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition-delete.md)|Нет|Удаляет [объект deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).|
|[Обновление объекта deviceManagementConfigurationSettingDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition-update.md)|[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|Обновление свойств объекта [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Применимость|[deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|Сведения о том, какой параметр устройства применим к|
|accessTypes|[deviceManagementConfigurationSettingAccessTypes](../resources/intune-shared-devicemanagementconfigurationsettingaccesstypes.md)|Режим доступа для чтения и записи параметра. Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.|
|keywords|Коллекция объектов string|Токены, на которых выполняется поиск параметров|
|infoUrls|Коллекция String|Список ссылок на дополнительные сведения о параметре можно найти по адресу|
|Вхождение|[deviceManagementConfigurationSettingOccurrence](../resources/intune-shared-devicemanagementconfigurationsettingoccurrence.md)|Указывает, является ли параметр обязательным или нет.|
|Baseuri|String|Базовый путь CSP|
|offsetUri|String|Смещение пути CSP от базового|
|rootDefinitionId|String|Определение корневого параметра, если параметр является дочерним.|
|Categoryid|String|Указывает группу с областями, в которой настроен параметр в указанном поставщике служб конфигурации (CSP).|
|settingUsage|[deviceManagementConfigurationSettingUsage](../resources/intune-shared-devicemanagementconfigurationsettingusage.md)|Тип параметра, например конфигурация и соответствие. Возможные значения: `none`, `configuration`, `compliance`.|
|uxBehavior|[DeviceManagementConfigurationControlType](../resources/intune-shared-devicemanagementconfigurationcontroltype.md)|Задание представления типа элемента управления в пользовательском интерфейсе. Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.|
|visibility|[deviceManagementConfigurationSettingVisibility](../resources/intune-shared-devicemanagementconfigurationsettingvisibility.md)|Настройка области видимости для пользовательского интерфейса. Возможные значения: `none`, `settingsCatalog`, `template`.|
|referredSettingInformationList|[Коллекция deviceManagementConfigurationReferredSettingInformation](../resources/intune-shared-devicemanagementconfigurationreferredsettinginformation.md)|Список ссылаемой информации о параметрах.|
|id|String|Идентификатор элемента|
|description|String|Описание элемента|
|Helptext|String|Текст справки элемента|
|name|String|Имя элемента|
|displayName|String|Отображаемое имя элемента|
|version|String|Версия элемента|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingDefinition",
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
  "visibility": "String",
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "String"
    }
  ],
  "id": "String (identifier)",
  "description": "String",
  "helpText": "String",
  "name": "String",
  "displayName": "String",
  "version": "String"
}
```




