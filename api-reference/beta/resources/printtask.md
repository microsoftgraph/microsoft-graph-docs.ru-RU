---
title: Тип ресурса printTask
description: Представляет задачу, которая выполняется или была выполнена в результате события универсальной печати.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 4348a07af0849359c72c6b28fa5ef665420a2842
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176750"
---
# <a name="printtask-resource-type"></a>Тип ресурса printTask

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет задачу, которая выполняется или была выполнена в результате события универсальной печати.

Дополнительные сведения об использовании этого ресурса для добавления поддержки печати по запросу в универсальную печать см. в разделе "Расширение универсальной печати для [поддержки печати по запросу"](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [List (from printTaskDefintion)](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | Получение списка задач, созданных на основе определенного объекта printTaskDefinition. Список включает в себя выполняющиеся задачи и недавно завершенные задачи. |
| [получение](../api/printtask-get.md); | [printTask](printtask.md) | Получение сведений о задаче печати. |
| [Обновление](../api/printtaskdefinition-update-task.md) | [printTask](printtask.md) | Обновляет задачу печати. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор printTask. Только для чтения.|
|status|[printTaskStatus](printtaskstatus.md)|Текущее состояние выполнения этого объекта printTask. **Вызывающее приложение отвечает за обновление этого состояния после завершения обработки, если связанное задание печати не было перенаправлено на другой принтер.** Если не сообщить о завершении, связанное задание печати будет заблокировано и в конечном итоге удалено. |
|parentUrl|Строка|URL-адрес сущности печати, которая активирует эту задачу. Например, `https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|Триггер|[printTaskTrigger](printtasktrigger.md)|PrintTaskTrigger, который инициирует выполнение этой задачи. Только для чтения.|
|Определение|[printTaskDefinition](printtaskdefinition.md)|PrintTaskDefinition, который использовался для создания этой задачи. Только для чтения.|

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


