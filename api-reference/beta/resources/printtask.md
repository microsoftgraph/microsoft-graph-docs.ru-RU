---
title: тип ресурса printTask
description: Представляет задачу, выполненную или выполненную в результате события универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c684ff64aa4c3667214b61b70a422690381525b3
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766303"
---
# <a name="printtask-resource-type"></a>тип ресурса printTask

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет задачу, выполненную или выполненную в результате события универсальной печати.

Дополнительные сведения о том, как использовать этот ресурс для добавления поддержки печати в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список (от printTaskDefintion)](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | Получите список задач, созданных на основе определенного шрифтаTaskDefinition. Список включает в себя выполнение текущих задач и недавно завершенных задач. |
| [Get](../api/printtask-get.md) | [printTask](printtask.md) | Сведения о задаче печати. |
| [Обновление](../api/printtaskdefinition-update-task.md) | [printTask](printtask.md) | Обновляет задачу печати. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор printTask. Только для чтения.|
|status|[printTaskStatus](printtaskstatus.md)|Текущее состояние выполнения этого printTask. **Приложение вызовов отвечает за обновление этого состояния по завершению обработки, если соответствующий printJob не был перенаправлен на другой принтер.** Невыполнение отчетов о завершении приведет к блокировке связанного задания печати от печати и в конечном итоге к их удаляемой работе. |
|parentUrl|String|URL-адрес для объекта печати, который вызвал эту задачу. Например, `https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|триггер|[printTaskTrigger](printtasktrigger.md)|PrintTaskTrigger, который вызвал выполнение этой задачи. Только для чтения.|
|определение|[printTaskDefinition](printtaskdefinition.md)|PrintTaskDefinition, который использовался для создания этой задачи. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTask",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "status": {"@odata.type": "microsoft.graph.printTaskStatus"},
  "parentUrl": "String",
  "trigger": {"@odata.type": "microsoft.graph.printTaskTrigger"},
  "definition": {"@odata.type": "microsoft.graph.printTaskDefinition"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


