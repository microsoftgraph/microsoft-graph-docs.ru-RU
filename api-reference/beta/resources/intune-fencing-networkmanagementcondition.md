---
title: Тип ресурса Нетворкманажементкондитион
description: Содержит сведения для определения условия управления сетью.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 909eaa89a8303948cd97ba47299146b575e32c9f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164836"
---
# <a name="networkmanagementcondition-resource-type"></a>Тип ресурса Нетворкманажементкондитион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит сведения для определения условия управления сетью.


НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Нетворкманажементкондитионс](../api/intune-fencing-networkmanagementcondition-list.md)|Коллекция [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md)|Список свойств и связей объектов [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md) .|
|[Получение Нетворкманажементкондитион](../api/intune-fencing-networkmanagementcondition-get.md)|[Нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md)|Чтение свойств и связей объекта [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для условия управления. Созданное системой значение, назначаемое при создании. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|uniqueName|String|Уникальное имя условия управления. Используется в выражениях условия управления. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|displayName|String|Имя условия управления, определенное администратором. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|description|Строка|Описание условия управления, заданное администратором. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Время создания условия управления. Созданная сторона службы. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Время последнего изменения условия управления. Обновленная сторона службы. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|eTag|String|Тег ETag условия управления. Обновленная сторона службы. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|Аппликаблеплатформс|Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)|Соответствующие платформы для этого условия управления. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|Манажементкондитионстатементс|Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)|Операторы условия управления, связанные с условием управления. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```




