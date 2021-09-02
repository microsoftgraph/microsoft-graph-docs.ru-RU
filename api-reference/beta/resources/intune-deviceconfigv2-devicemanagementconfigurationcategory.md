---
title: тип ресурса deviceManagementConfigurationCategory
description: Политика конфигурации управления устройствами
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 60850512e44de514892fcd998962e7a37197d343
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58784830"
---
# <a name="devicemanagementconfigurationcategory-resource-type"></a>тип ресурса deviceManagementConfigurationCategory

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политика конфигурации управления устройствами

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementConfigurationCategories](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-list.md)|[коллекция deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|Список свойств и связей [объектов deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|
|[Get deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-get.md)|[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|Чтение свойств и связей [объекта deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|
|[Создание deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-create.md)|[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|Создание нового [объекта deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|
|[Удаление deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-delete.md)|Нет|Удаляет [устройствоManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md).|
|[Обновление deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-update.md)|[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|Обновление свойств объекта [deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор элемента|
|description|Строка|Описание элемента|
|helpText|Строка|Справка текста элемента|
|name|String|Имя элемента|
|displayName|Строка|Отображение имени элемента|
|платформы|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Типы платформ, которые имеются в этой категории. Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.|
|технологии|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Типы технологий, которые имеют параметры в категории. Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`, `exchangeOnline`.|
|settingUsage|[deviceManagementConfigurationSettingUsage](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|Указывает, что категория содержит параметры, используемые для соответствия требованиям или конфигурации. Возможные значения: `none`, `configuration`.|
|parentCategoryId|Строка|Родительский id категории.|
|rootCategoryId|Строка|Корневой id категории.|
|childCategoryIds|Коллекция String|Список детских ids этой категории.|

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



