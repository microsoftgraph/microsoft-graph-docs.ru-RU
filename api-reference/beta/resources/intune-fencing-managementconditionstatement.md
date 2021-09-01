---
title: тип ресурса managementConditionStatement
description: Заявление об условиях управления — это группа условий управления, которые позволяют/отключать конфигурации устройств и приложений при условии, что все условия управления выполнены.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 367739eb54144b29fc0d109174f2d89108418d0b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58769483"
---
# <a name="managementconditionstatement-resource-type"></a>тип ресурса managementConditionStatement

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Заявление об условиях управления — это группа условий управления, которые позволяют/отключать конфигурации устройств и приложений при условии, что все условия управления выполнены.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Управление спискамиConditionStatements](../api/intune-fencing-managementconditionstatement-list.md)|[коллекция managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Список свойств и связей объектов [managementConditionStatement.](../resources/intune-fencing-managementconditionstatement.md)|
|[Get managementConditionStatement](../api/intune-fencing-managementconditionstatement-get.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Чтение свойств и связей [объекта managementConditionStatement.](../resources/intune-fencing-managementconditionstatement.md)|
|[Создание managementConditionStatement](../api/intune-fencing-managementconditionstatement-create.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Создание нового [объекта managementConditionStatement.](../resources/intune-fencing-managementconditionstatement.md)|
|[Удаление управленияConditionStatement](../api/intune-fencing-managementconditionstatement-delete.md)|Нет|Удаляет [управлениеConditionStatement](../resources/intune-fencing-managementconditionstatement.md).|
|[Update managementConditionStatement](../api/intune-fencing-managementconditionstatement-update.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Обновление свойств объекта [managementConditionStatement.](../resources/intune-fencing-managementconditionstatement.md)|
|[функция getManagementConditionStatementExpressionString](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md)|Пока не задокументировано.|
|[функция getManagementConditionStatementsForPlatform](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|[коллекция managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для утверждения условий управления. Созданное в системе значение, назначенное при его создания.|
|displayName|Строка|Администратор определил имя заявления об условиях управления.|
|description|Строка|Администратор определил описание инструкции по состоянию управления.|
|createdDateTime|DateTimeOffset|Время создания заявления об условиях управления. Сгенерированная сторона службы.|
|modifiedDateTime|DateTimeOffset|Время последнего изменения состояния управления. Обновленная сторона службы.|
|выражение|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|Выражение заявления об условиях управления, используемое для оценки активации или отключения заявления об условиях управления.|
|eTag|String|ETag заявления об условиях управления. Обновленная сторона службы.|
|applicablePlatforms|[коллекция devicePlatformType](../resources/intune-fencing-deviceplatformtype.md)|Применимые платформы для этого утверждения условий управления.
Это рассчитывается из поиска условий управления, связанных с утверждением условий управления и поиска пересечения применимых платформ.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managementConditions|[коллекция managementCondition](../resources/intune-fencing-managementcondition.md)|Условия управления, связанные с утверждением условий управления.|

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
    "@odata.type": "microsoft.graph.managementConditionExpressionString",
    "value": "String"
  },
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```



