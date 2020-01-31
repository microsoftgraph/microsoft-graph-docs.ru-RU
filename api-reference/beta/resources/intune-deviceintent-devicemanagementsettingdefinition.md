---
title: Тип ресурса Девицеманажементсеттингдефинитион
description: Сущность, представляющая определение определения для заданной настройки
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2f5774a220edd9113425801364bdca7df4982cfe
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636800"
---
# <a name="devicemanagementsettingdefinition-resource-type"></a>Тип ресурса Девицеманажементсеттингдефинитион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляющая определение определения для заданной настройки

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементсеттингдефинитионс](../api/intune-deviceintent-devicemanagementsettingdefinition-list.md)|Коллекция [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Список свойств и связей объектов [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .|
|[Получение Девицеманажементсеттингдефинитион](../api/intune-deviceintent-devicemanagementsettingdefinition-get.md)|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Чтение свойств и связей объекта [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .|
|[Создание Девицеманажементсеттингдефинитион](../api/intune-deviceintent-devicemanagementsettingdefinition-create.md)|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Создание нового объекта [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .|
|[Удаление Девицеманажементсеттингдефинитион](../api/intune-deviceintent-devicemanagementsettingdefinition-delete.md)|Нет|Удаляет объект [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).|
|[Обновление Девицеманажементсеттингдефинитион](../api/intune-deviceintent-devicemanagementsettingdefinition-update.md)|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Обновление свойств объекта [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор определения параметра|
|Типом|[deviceManangementIntentValueType](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|Тип данных значения. Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.|
|displayName|Строка|Отображаемое имя параметра|
|истоплевел|Boolean|Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр.|
|description|String|Описание параметра|
|плацехолдертекст|Строка|Замещающий текст в качестве примера допустимых входных данных|
|документатионурл|Строка|URL-адрес для установки документации|
|keywords|Коллекция String|Ключевые слова, связанные с параметром|
|провероч|Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)|Коллекция ограничений для значения параметра|
|зависящ|Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)|Коллекция зависимостей для других параметров|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "String (identifier)",
  "valueType": "String",
  "displayName": "String",
  "isTopLevel": true,
  "description": "String",
  "placeholderText": "String",
  "documentationUrl": "String",
  "keywords": [
    "String"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "String"
      ]
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "String",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
          "supportedTypes": [
            "String"
          ]
        }
      ]
    }
  ]
}
```



