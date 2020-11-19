---
title: Тип ресурса Девицеманажементконфигуратионсеттингдефинитион
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7d5e0b2e1c200ffb14011d7fcd22aac3aca86246
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242187"
---
# <a name="devicemanagementconfigurationsettingdefinition-resource-type"></a>Тип ресурса Девицеманажементконфигуратионсеттингдефинитион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементконфигуратионсеттингдефинитионс](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition-list.md)|Коллекция [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|Список свойств и связей объектов [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) .|
|[Получение Девицеманажементконфигуратионсеттингдефинитион](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition-get.md)|[девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|Чтение свойств и связей объекта [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) .|
|[Создание Девицеманажементконфигуратионсеттингдефинитион](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition-create.md)|[девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|Создание нового объекта [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) .|
|[Удаление Девицеманажементконфигуратионсеттингдефинитион](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition-delete.md)|Нет|Удаляет объект [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).|
|[Обновление Девицеманажементконфигуратионсеттингдефинитион](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition-update.md)|[девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|Обновление свойств объекта [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|применения|[девицеманажементконфигуратионсеттингаппликабилити](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|Сведения о том, какие параметры устройства применяются для|
|акцесстипес|[девицеманажементконфигуратионсеттингакцесстипес](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|Режим доступа для чтения и записи параметра. Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.|
|keywords|Коллекция строк|Маркеры, для которых необходимо выполнить поиск параметров|
|инфаурлс|Коллекция строк|Список ссылок дополнительные сведения для параметра можно найти по адресу|
|экземпляр|[девицеманажементконфигуратионсеттингоккурренце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|Указывает, является ли параметр обязательным или нет|
|baseUri|String|Путь к основному поставщику служб шифрования|
|оффсетури|String|Путь от базового поставщика CSP|
|рутдефинитионид|String|Определение корневого параметра, если параметр является дочерним.|
|categoryId|String|Указывает группу областей, в которой параметр настроен в указанном поставщике службы конфигурации (CSP).|
|сеттингусаже|[девицеманажементконфигуратионсеттингусаже](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|Тип параметра, например, "Конфигурация" и "соответствие". Возможные значения: `none`, `configuration`.|
|id|String|Идентификатор элемента|
|description|String|Описание элемента|
|helpText|String|Текст справки элемента|
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
  "id": "String (identifier)",
  "description": "String",
  "helpText": "String",
  "name": "String",
  "displayName": "String",
  "version": "String"
}
```




