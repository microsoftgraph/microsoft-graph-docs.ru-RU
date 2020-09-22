---
title: Тип ресурса Принттаскдефинитион
description: Представляет задачу, которая может быть активирована при возникновении различных событий в рамках универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 970b4169dcf4d94eed01be7a15654daa51760151
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078313"
---
# <a name="printtaskdefinition-resource-type"></a>Тип ресурса Принттаскдефинитион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет абстрактное определение задачи, которое может быть запущено при возникновении различных событий в рамках универсальной печати.

Дополнительные сведения о том, как использовать этот ресурс для поддержки печати по запросу в универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/print-list-taskdefinitions.md) | Коллекция [принттаскдефинитион](printtaskdefinition.md) | Получение полного списка Принттаскдефинитионс, созданных в рамках универсальной печати. |
| [Создание](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | Создание нового Принттаскдефинитион. |
| [Обновление](../api/print-update-taskdefinition.md) | [printTaskDefinition](printtaskdefinition.md) | Обновление Принттаскдефинитион. |
| [Удаление](../api/print-delete-taskdefinition.md) | Нет | Удаление объекта Принттаскдефинитион. |
| [Перечисление задач](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | Получение списка задач, созданных на основе этого определения. Список содержит текущие выполняемые задачи и недавно выполненные задачи. |
| [Вывод задачи](../api/printtask-get.md) | [printTask](printtask.md) | Получает задачу, созданную на основе этого определения. |
| [Обновление задачи](../api/printtaskdefinition-update-task.md) | Нет | Обновление задачи, созданной на основе этого определения. **Приложения, которые регистрируют триггеры задач, несут ответственность за обновление состояния задачи при завершении обработки, если связанный метод printJob не будет перенаправлен на другой принтер.** Если не выполнить отчет о завершении, то соответствующее задание печати блокируется для печати и в конечном итоге удалено. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор Принттаскдефинитион. Только для чтения.|
|displayName|String|Имя Принттаскдефинитион.|
|createdBy|[аппидентити](appidentity.md)|Приложение, создавшее Принттаскдефинитион. Только для чтения.|

## <a name="relationships"></a>Отношения
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|tasks|Коллекция [принттаск](printtask.md)|Список задач, созданных на основе этого определения. Список содержит текущие выполняемые задачи и недавно выполненные задачи. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "createdBy": {"@odata.type": "microsoft.graph.appIdentity"},
  "tasks": [{"@odata.type": "microsoft.graph.printTask"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

