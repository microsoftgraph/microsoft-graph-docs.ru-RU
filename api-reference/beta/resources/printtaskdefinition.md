---
title: тип ресурса printTaskDefinition
description: Представляет задачу, которая может быть вызвана при различных событиях, происходящих в универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 2495825ec64d73bb440d16e4eae9125f8dbd38eb
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766310"
---
# <a name="printtaskdefinition-resource-type"></a>тип ресурса printTaskDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет абстрактное определение задачи, которая может быть вызвана при различных событиях, происходящих в универсальной печати.

Дополнительные сведения о том, как использовать этот ресурс для добавления поддержки печати в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)

Этот ресурс поддерживает:
* [Подписка на изменение уведомлений.](/graph/universal-print-webhook-notifications)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/print-list-taskdefinitions.md) | [printTaskDefinition collection](printtaskdefinition.md) | Получите полный список отпечатковTaskDefinitions, созданных в универсальной печати. |
| [Create](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | Создайте новый шрифтTaskDefinition. |
| [Обновление](../api/print-update-taskdefinition.md) | [printTaskDefinition](printtaskdefinition.md) | Обновление печатиTaskDefinition. |
| [Delete](../api/print-delete-taskdefinition.md) | Нет | Удаление печатиTaskDefinition. |
| [Перечисление задач](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | Получите список задач, созданных на основе этого определения. Список включает в себя выполнение текущих задач и недавно завершенных задач. |
| [Вывод задачи](../api/printtask-get.md) | [printTask](printtask.md) | Получает задачу, созданную на основе этого определения. |
| [Обновление задачи](../api/printtaskdefinition-update-task.md) | [printTask](printtask.md) | Обновление задачи, созданной на основе этого определения. **Приложения, которые регистрируют триггеры задач, отвечают за обновление состояния задачи по завершению обработки, если соответствующий printJob не был перенаправлен на другой принтер.** Невыполнение отчетов о завершении приведет к блокировке связанного задания печати от печати и в конечном итоге к их удаляемой работе. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор printTaskDefinition. Только для чтения.|
|displayName|String|Имя печатиTaskDefinition.|
|createdBy|[appIdentity](appidentity.md)|Приложение, создав печатьTaskDefinition. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|tasks|[printTask](printtask.md) collection|Список задач, созданных на основе этого определения. Список включает в себя выполнение текущих задач и недавно завершенных задач. Только для чтения.|

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

