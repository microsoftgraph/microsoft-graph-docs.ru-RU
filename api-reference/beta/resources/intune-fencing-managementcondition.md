---
title: Тип ресурса managementCondition
description: События, например географически границы, может быть запущено динамически выполняются условия управления временные границы и границы сети.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: e0aeb73a93cd4c61b6d4680f73c2a9b8cee830c6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986744"
---
# <a name="managementcondition-resource-type"></a>Тип ресурса managementCondition

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

События, например географически границы, может быть запущено динамически выполняются условия управления временные границы и границы сети.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список managementConditions](../api/intune-fencing-managementcondition-list.md)|[managementCondition](../resources/intune-fencing-managementcondition.md) коллекции|Свойства списка и связей объектов [managementCondition](../resources/intune-fencing-managementcondition.md) .|
|[Получение managementCondition](../api/intune-fencing-managementcondition-get.md)|[managementCondition](../resources/intune-fencing-managementcondition.md)|Чтение свойства и связи объекта [managementCondition](../resources/intune-fencing-managementcondition.md) .|
|[функция getManagementConditionsForPlatform](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|[managementCondition](../resources/intune-fencing-managementcondition.md) коллекции|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для управления условия. Значение, назначенное при создании создаваемый системой.|
|уникального имени|Строка|Уникальное имя для управления условия. Используется в выражениях условие управления.|
|displayName|Строка|Имя условия управления определенные администратором.|
|описание|Строка|Описание управления условия, определенные администратором.|
|createdDateTime|DateTimeOffset|Время создания условие управления. Создан со стороны службы.|
|modifiedDateTime|DateTimeOffset|Время последнего изменения условие управления. Обновление со стороны службы.|
|eTag|String|ETag условие управления. Обновление со стороны службы.|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции|Применимые платформ для этого условия управления.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) коллекции|Операторы условие управления, связанные с условием управления.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCondition",
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





