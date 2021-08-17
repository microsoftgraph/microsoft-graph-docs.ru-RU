---
title: тип ресурса circularGeofenceManagementCondition
description: Содержит сведения для определения состояния управления круговым геограждением, интересуемого для мониторинга.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b98ed0e12fc726417c10904bff0783fdb9cf1aea
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58264670"
---
# <a name="circulargeofencemanagementcondition-resource-type"></a>тип ресурса circularGeofenceManagementCondition

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит сведения для определения состояния управления круговым геограждением, интересуемого для мониторинга.


Наследует от [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список circularGeofenceManagementConditions](../api/intune-fencing-circulargeofencemanagementcondition-list.md)|[коллекция circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Список свойств и связей объектов [circularGeofenceManagementCondition.](../resources/intune-fencing-circulargeofencemanagementcondition.md)|
|[Get circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-get.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Чтение свойств и связей объекта [circularGeofenceManagementCondition.](../resources/intune-fencing-circulargeofencemanagementcondition.md)|
|[Создание circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-create.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Создайте новый [объект circularGeofenceManagementCondition.](../resources/intune-fencing-circulargeofencemanagementcondition.md)|
|[Удаление circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-delete.md)|Нет|Удаляет [циркулярGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).|
|[Обновление циркуляраGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-update.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Обновление свойств объекта [circularGeofenceManagementCondition.](../resources/intune-fencing-circulargeofencemanagementcondition.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для состояния управления. Созданное в системе значение, назначенное при его создания. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|uniqueName|Строка|Уникальное имя для состояния управления. Используется в выражениях условий управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|String|Администратор определил имя условия управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|String|Администратор определил описание условия управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Время создания условия управления. Сгенерированная сторона службы. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Время последнего изменения условия управления. Обновленная сторона службы. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag состояния управления. Обновленная сторона службы. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[коллекция devicePlatformType](../resources/intune-fencing-deviceplatformtype.md)|Применимые платформы для этого условия управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|latitude|Double|Широта в градусах, от -90 до +90 включительно.|
|longitude|Double|Долгота в градусах, от -180 до +180 включительно.|
|radiusInMeters|Один|Радиус в метрах.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managementConditionStatements|[коллекция managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Утверждения условий управления, связанные с состоянием управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|

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
  "latitude": "4.2",
  "longitude": "4.2",
  "radiusInMeters": 4.2
}
```




