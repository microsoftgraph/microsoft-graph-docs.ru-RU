---
title: Тип ресурса Девицеманажементконфигуратионсеттингграупдефинитион
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 439dce34f2e536a94a591328002cd172d9743507
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242179"
---
# <a name="devicemanagementconfigurationsettinggroupdefinition-resource-type"></a>Тип ресурса Девицеманажементконфигуратионсеттингграупдефинитион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.


Наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементконфигуратионсеттингграупдефинитионс](../api/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition-list.md)|Коллекция [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)|Список свойств и связей объектов [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) .|
|[Получение Девицеманажементконфигуратионсеттингграупдефинитион](../api/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition-get.md)|[девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)|Чтение свойств и связей объекта [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) .|
|[Создание Девицеманажементконфигуратионсеттингграупдефинитион](../api/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition-create.md)|[девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)|Создание нового объекта [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) .|
|[Удаление Девицеманажементконфигуратионсеттингграупдефинитион](../api/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition-delete.md)|Нет|Удаляет объект [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md).|
|[Обновление Девицеманажементконфигуратионсеттингграупдефинитион](../api/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition-update.md)|[девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)|Обновление свойств объекта [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|применения|[девицеманажементконфигуратионсеттингаппликабилити](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|Сведения о том, какие параметры устройства применяются в унаследованном от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|акцесстипес|[девицеманажементконфигуратионсеттингакцесстипес](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|Режим доступа для чтения и записи параметра, унаследованного от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md). Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.|
|keywords|Коллекция строк|Маркеры, для которых параметры поиска унаследованы от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|инфаурлс|Коллекция строк|Список ссылок дополнительные сведения для параметра можно найти в разделе унаследовано от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|экземпляр|[девицеманажементконфигуратионсеттингоккурренце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|Указывает, является ли параметр обязательным или не наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|baseUri|String|Базовый путь поставщика CSP наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|оффсетури|String|Путь к поставщику службы шифрования из базового наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|рутдефинитионид|String|Определение корневого параметра, если параметр является дочерним. Наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|categoryId|String|Указывает группу областей, в которой параметр настроен в указанном поставщике службы конфигурации (CSP), унаследованном от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|сеттингусаже|[девицеманажементконфигуратионсеттингусаже](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|Тип параметра, например конфигурация и соответствие, наследуемые от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md). Возможные значения: `none`, `configuration`.|
|id|String|Идентификатор элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|description|String|Описание элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|helpText|String|Текст справки элемента, наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|name|String|Имя элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|displayName|String|Отображаемое имя элемента, наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|version|String|Версия элемента наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|чилдидс|Коллекция строк|Зависимые параметры дочерних элементов для этой группы параметров|
|депендентон|Коллекция [девицеманажементконфигуратиондепендентон](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)|Список зависимостей для группы параметров|
|депендедонби|Коллекция [девицеманажементконфигуратионсеттингдепендедонби](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)|Список дочерних параметров, зависящих от этого параметра|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingGroupDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupDefinition",
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
  ]
}
```




