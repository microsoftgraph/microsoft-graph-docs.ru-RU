---
title: Тип ресурса circularGeofenceManagementCondition
description: Содержит данные для определения условие управления циклическое географическая граница области интересов, мониторинг.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 641e87a623d20f7290b58180266030c58518e384
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422098"
---
# <a name="circulargeofencemanagementcondition-resource-type"></a>Тип ресурса circularGeofenceManagementCondition

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит данные для определения условие управления циклическое географическая граница области интересов, мониторинг.


Наследуется от [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список circularGeofenceManagementConditions](../api/intune-fencing-circulargeofencemanagementcondition-list.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) коллекции|Свойства списка и связей объектов [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .|
|[Получение circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-get.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Чтение свойства и связи объекта [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .|
|[Создание circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-create.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Создание нового объекта [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .|
|[Удаление circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-delete.md)|Нет|Удаляет [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).|
|[Обновление circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-update.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Обновление свойства объекта [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для управления условия. Значение, назначенное при создании создаваемый системой. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|уникального имени|String|Уникальное имя для управления условия. Используется в выражениях условие управления. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|String|Имя условия управления определенные администратором. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|String|Описание управления условия, определенные администратором. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Время создания условие управления. Создан со стороны службы. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Время последнего изменения условие управления. Обновление со стороны службы. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag условие управления. Обновление со стороны службы. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции|Применимые платформ для этого условия управления. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|latitude|Double|Широта в степени, от -90 до 90 включительно.|
|longitude|Double|Долгота в градусов между -180 и + 180 включительно.|
|radiusInMeters|Single|RADIUS в метры.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) коллекции|Операторы условие управления, связанные с условием управления. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|

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




