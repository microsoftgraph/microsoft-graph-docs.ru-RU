---
title: Тип ресурса networkManagementCondition
description: Содержит данные для определения состояния управления сети.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7d91ac60ae52f3317e8148e8bb4adcaf82afac53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806512"
---
# <a name="networkmanagementcondition-resource-type"></a>Тип ресурса networkManagementCondition

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит данные для определения состояния управления сети.

Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список networkManagementConditions](../api/intune-fencing-networkmanagementcondition-list.md)|[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) коллекции|Свойства списка и связей объектов [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .|
|[Получение networkManagementCondition](../api/intune-fencing-networkmanagementcondition-get.md)|[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)|Чтение свойства и связи объекта [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для управления условия. Значение, назначенное при создании создаваемый системой. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|уникального имени|Строка|Уникальное имя для управления условия. Используется в выражениях условие управления. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|Строка|Имя условия управления определенные администратором. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|описание|Строка|Описание управления условия, определенные администратором. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Время создания условие управления. Создан со стороны службы. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Время последнего изменения условие управления. Обновление со стороны службы. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag условие управления. Обновление со стороны службы. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции|Применимые платформ для этого условия управления. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) коллекции|Операторы условие управления, связанные с условием управления. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|

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





