---
title: Тип ресурса managementConditionStatement
description: Условная инструкция управления — это группа управления условий, включения или отключения конфигурации устройства или приложение при все содержащиеся управления условий.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 82a99e878337cf04659b8bc7da7e821bd8afb6aa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929986"
---
# <a name="managementconditionstatement-resource-type"></a>Тип ресурса managementConditionStatement

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Условная инструкция управления — это группа управления условий, включения или отключения конфигурации устройства или приложение при все содержащиеся управления условий.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список managementConditionStatements](../api/intune-fencing-managementconditionstatement-list.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) коллекции|Свойства списка и связей объектов [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .|
|[Получение managementConditionStatement](../api/intune-fencing-managementconditionstatement-get.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Чтение свойства и связи объекта [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .|
|[Создание managementConditionStatement](../api/intune-fencing-managementconditionstatement-create.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Создание нового объекта [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .|
|[Удаление managementConditionStatement](../api/intune-fencing-managementconditionstatement-delete.md)|Нет|Удаляет [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).|
|[Обновление managementConditionStatement](../api/intune-fencing-managementconditionstatement-update.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Обновление свойства объекта [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .|
|[функция getManagementConditionStatementExpressionString](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md)|Н/Д|
|[функция getManagementConditionStatementsForPlatform](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) коллекции|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для управления условная инструкция. Значение, назначенное при создании создаваемый системой.|
|displayName|Строка|Имя оператора условия управления определенные администратором.|
|описание|Строка|Описание управления условная инструкция определенные администратором.|
|createdDateTime|DateTimeOffset|Время создания условная инструкция управления. Создан со стороны службы.|
|modifiedDateTime|DateTimeOffset|Время последнего изменения условная инструкция управления. Обновление со стороны службы.|
|выражение|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|Выражение оператора условия управления, используется для оценки Если инструкции с условием управления был активирован деактивирован.|
|eTag|String|ETag условная инструкция управления. Обновление со стороны службы.|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции|Применимые платформы для этой условная инструкция управления.
Отсчитывается от нужна условия управления, связанные с управлением условие оператора и поиск пересечения применимых платформ.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managementConditions|[managementCondition](../resources/intune-fencing-managementcondition.md) коллекции|Условия управления, связанный со условная инструкция управления.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementConditionStatement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```





