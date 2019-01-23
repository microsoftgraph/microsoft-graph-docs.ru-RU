---
title: Тип ресурса managementConditionStatement
description: Условная инструкция управления — это группа управления условий, включения или отключения конфигурации устройства или приложение при все содержащиеся управления условий.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3292dae241a3f79cc7d3417c93ccc1187c8b8d17
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395995"
---
# <a name="managementconditionstatement-resource-type"></a>Тип ресурса managementConditionStatement

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|String|Уникальный идентификатор для управления условная инструкция. Значение, назначенное при создании создаваемый системой.|
|displayName|String|Имя оператора условия управления определенные администратором.|
|description|String|Описание управления условная инструкция определенные администратором.|
|createdDateTime|DateTimeOffset|Время создания условная инструкция управления. Создан со стороны службы.|
|modifiedDateTime|DateTimeOffset|Время последнего изменения условная инструкция управления. Обновление со стороны службы.|
|выражение|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|Выражение оператора условия управления, используется для оценки Если инструкции с условием управления был активирован деактивирован.|
|eTag|String|ETag условная инструкция управления. Обновление со стороны службы.|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции|Применимые платформы для этой условная инструкция управления.
Отсчитывается от нужна условия управления, связанные с управлением условие оператора и поиск пересечения применимых платформ.|

## <a name="relationships"></a>Отношения
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




