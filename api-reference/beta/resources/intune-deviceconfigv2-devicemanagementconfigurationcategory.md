---
title: Тип ресурса deviceManagementConfigurationCategory
description: Управление устройствами конфигурации
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fd8bf0c4f5102f9338673a7b0fdea6f1cc78b5a0
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202765"
---
# <a name="devicemanagementconfigurationcategory-resource-type"></a>Тип ресурса deviceManagementConfigurationCategory

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Управление устройствами конфигурации

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление deviceManagementConfigurationCategories](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-list.md)|[Коллекция deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|Список свойств и связей объектов [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) .|
|[Получение объекта deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-get.md)|[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|Чтение свойств и связей объекта [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) .|
|[Создание объекта deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-create.md)|[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|Создайте объект [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) .|
|[Удаление объекта deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-delete.md)|Нет|Удаляет [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md).|
|[Обновление объекта deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-update.md)|[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|Обновление свойств объекта [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор элемента|
|description|Строка|Описание элемента|
|categoryDescription|String|Описание заголовка категории|
|Helptext|String|Текст справки элемента|
|name|String|Имя элемента|
|displayName|Строка|Отображаемое имя элемента|
|Платформ|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Типы платформ, которые имеют параметры в категории. Возможные значения: `none`, `android`, `iOS`, `macOS`, `windows10X`, `windows10`, `linux`, `unknownFutureValue`.|
|Технологии|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Типы технологий, параметры которых имеются в категории. Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`, `appleRemoteManagement`, `microsoftSense`, `exchangeOnline`, `linuxMdm`, `unknownFutureValue`.|
|settingUsage|[deviceManagementConfigurationSettingUsage](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|Указывает, что категория содержит параметры, используемые для соответствия или конфигурации. Возможные значения: `none`, `configuration`, `compliance`.|
|parentCategoryId|Строка|Родительский идентификатор категории.|
|rootCategoryId|Строка|Корневой идентификатор категории.|
|childCategoryIds|Коллекция строк|Список дочерних идентификаторов категории.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "id": "String (identifier)",
  "description": "String",
  "categoryDescription": "String",
  "helpText": "String",
  "name": "String",
  "displayName": "String",
  "platforms": "String",
  "technologies": "String",
  "settingUsage": "String",
  "parentCategoryId": "String",
  "rootCategoryId": "String",
  "childCategoryIds": [
    "String"
  ]
}
```




