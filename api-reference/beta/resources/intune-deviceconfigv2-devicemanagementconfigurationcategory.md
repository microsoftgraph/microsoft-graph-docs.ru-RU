---
title: Тип ресурса Девицеманажементконфигуратионкатегори
description: Политика конфигурации управления устройствами
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e2225f24aab8f969a142afdfa1b1aa9ceca9f309
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302038"
---
# <a name="devicemanagementconfigurationcategory-resource-type"></a>Тип ресурса Девицеманажементконфигуратионкатегори

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политика конфигурации управления устройствами

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементконфигуратионкатегориес](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-list.md)|Коллекция [девицеманажементконфигуратионкатегори](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|Список свойств и связей объектов [девицеманажементконфигуратионкатегори](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) .|
|[Получение Девицеманажементконфигуратионкатегори](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-get.md)|[девицеманажементконфигуратионкатегори](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|Чтение свойств и связей объекта [девицеманажементконфигуратионкатегори](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) .|
|[Создание Девицеманажементконфигуратионкатегори](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-create.md)|[девицеманажементконфигуратионкатегори](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|Создание нового объекта [девицеманажементконфигуратионкатегори](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) .|
|[Удаление Девицеманажементконфигуратионкатегори](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-delete.md)|Нет|Удаляет объект [девицеманажементконфигуратионкатегори](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md).|
|[Обновление Девицеманажементконфигуратионкатегори](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-update.md)|[девицеманажементконфигуратионкатегори](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|Обновление свойств объекта [девицеманажементконфигуратионкатегори](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор элемента|
|description|String|Описание элемента|
|helpText|String|Текст справки элемента|
|name|String|Имя элемента|
|displayName|String|Отображаемое имя элемента|
|Embedded|[девицеманажементконфигуратионплатформс](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Типы платформ, которые имеют параметры в категории. Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.|
|технологически|[девицеманажементконфигуратионтечнологиес](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Типы технологий, которые имеют параметры в категории. Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`.|

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
  "technologies": "String"
}
```




