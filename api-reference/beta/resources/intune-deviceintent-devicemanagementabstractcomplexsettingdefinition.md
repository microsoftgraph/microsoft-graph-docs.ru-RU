---
title: Тип ресурса Девицеманажементабстракткомплекссеттингдефинитион
description: Сущность, представляющая определение абстрактного сложного параметра
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 840b4549c61e7d2f7b9f0fbd1c4a0c4df1142ea3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470832"
---
# <a name="devicemanagementabstractcomplexsettingdefinition-resource-type"></a>Тип ресурса Девицеманажементабстракткомплекссеттингдефинитион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляющая определение абстрактного сложного параметра


Наследуется от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементабстракткомплекссеттингдефинитионс](../api/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition-list.md)|Коллекция [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md)|Список свойств и связей объектов [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .|
|[Получение Девицеманажементабстракткомплекссеттингдефинитион](../api/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition-get.md)|[deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md)|Чтение свойств и связей объекта [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .|
|[Создание Девицеманажементабстракткомплекссеттингдефинитион](../api/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition-create.md)|[deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md)|Создание нового объекта [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .|
|[Удаление Девицеманажементабстракткомплекссеттингдефинитион](../api/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition-delete.md)|Нет|Удаляет объект [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md).|
|[Обновление Девицеманажементабстракткомплекссеттингдефинитион](../api/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition-update.md)|[deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md)|Обновление свойств объекта [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор определения параметра, унаследованного от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|Типом|[deviceManangementIntentValueType](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|Тип данных значения, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md). Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.|
|displayName|Строка|Отображаемое имя параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|истоплевел|Boolean|Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр, наследуемый от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|description|String|Описание параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|плацехолдертекст|String|Замещающий текст в качестве примера допустимых входных данных, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|документатионурл|String|URL-адрес для установки документации, унаследованной от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|keywords|Коллекция String|Ключевые слова, связанные с параметром, унаследованным от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|провероч|Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)|Коллекция ограничений для значения параметра, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|зависящ|Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)|Коллекция зависимостей от других параметров, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|реализации|Коллекция String|Список идентификаторов определений для всех возможных реализаций этого абстрактного сложного параметра|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementAbstractComplexSettingDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
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
  ],
  "implementations": [
    "String"
  ]
}
```



