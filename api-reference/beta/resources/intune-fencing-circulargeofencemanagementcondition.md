---
title: Тип ресурса Циркуларжеофенцеманажементкондитион
description: Содержит сведения о том, как определить циклическое условие управления для геоограждения, интересующее область мониторинга.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f826bd05a7f21df9ccf46579b77dc13967c31231
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568817"
---
# <a name="circulargeofencemanagementcondition-resource-type"></a>Тип ресурса Циркуларжеофенцеманажементкондитион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит сведения о том, как определить циклическое условие управления для геоограждения, интересующее область мониторинга.


НаСледуется от [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Циркуларжеофенцеманажементкондитионс](../api/intune-fencing-circulargeofencemanagementcondition-list.md)|Коллекция [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Список свойств и связей объектов [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) .|
|[Получение Циркуларжеофенцеманажементкондитион](../api/intune-fencing-circulargeofencemanagementcondition-get.md)|[Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Чтение свойств и связей объекта [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) .|
|[Создание Циркуларжеофенцеманажементкондитион](../api/intune-fencing-circulargeofencemanagementcondition-create.md)|[Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Создание нового объекта [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) .|
|[Удаление Циркуларжеофенцеманажементкондитион](../api/intune-fencing-circulargeofencemanagementcondition-delete.md)|Нет|Удаляет объект [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md).|
|[Обновление Циркуларжеофенцеманажементкондитион](../api/intune-fencing-circulargeofencemanagementcondition-update.md)|[Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Обновление свойств объекта [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для условия управления. Созданное системой значение, назначаемое при создании. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|uniqueName|String|Уникальное имя условия управления. Используется в выражениях условия управления. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|displayName|String|Имя условия управления, определенное администратором. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|description|String|Описание условия управления, заданное администратором. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Время создания условия управления. Созданная сторона службы. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Время последнего изменения условия управления. Обновленная сторона службы. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|eTag|String|Тег ETag условия управления. Обновленная сторона службы. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|Аппликаблеплатформс|Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)|Соответствующие платформы для этого условия управления. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|latitude|Double|Широта в градусах от – 90 до + 90 включительно.|
|longitude|Двойное|Долгота в градусах от – 180 до + 180 включительно.|
|Радиусинметерс|Одинарное|Радиус в метрах.|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|Манажементкондитионстатементс|Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)|Операторы условия управления, связанные с условием управления. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.circularGeofenceManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ],
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
}
```





