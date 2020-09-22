---
title: Тип ресурса Принттаск
description: Представляет задачу, которая выполняется или была выполнена в результате универсального события печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: fb41bc68112aa04e1eea825d45982f2f3f0db48c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973794"
---
# <a name="printtask-resource-type"></a>Тип ресурса Принттаск

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет задачу, которая выполняется или была выполнена в результате универсального события печати.

Дополнительные сведения о том, как использовать этот ресурс для поддержки печати по запросу в универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список (из Принттаскдефинтион)](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | Получение списка задач, созданных на основе определенного Принттаскдефинитион. Список содержит текущие выполняемые задачи и недавно выполненные задачи. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор Принттаск. Только для чтения.|
|status|[printTaskStatus](printtaskstatus.md)|Текущее состояние выполнения этого Принттаск. **Вызывающее приложение несет ответственность за обновление этого состояния после завершения обработки, если связанный с ним метод printJob не будет перенаправлен на другой принтер.** Если не выполнить отчет о завершении, то соответствующее задание печати блокируется для печати и в конечном итоге удалено. |
|parentUrl|String|URL-адрес объекта печати, который инициировал эту задачу. Например, `https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`. Только для чтения.|

## <a name="relationships"></a>Отношения
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|активирован|[printTaskTrigger](printtasktrigger.md)|Принттасктригжер, который инициировал выполнение этой задачи. Только для чтения.|
|RDLC|[printTaskDefinition](printtaskdefinition.md)|Принттаскдефинитион, который использовался для создания этой задачи. Только для чтения.|

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


