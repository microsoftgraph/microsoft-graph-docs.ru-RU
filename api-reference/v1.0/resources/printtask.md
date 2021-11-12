---
title: тип ресурса printTask
description: Представляет задачу, выполненную или выполненную в результате события универсальной печати.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 66229e5089026f22fa90f5db52c9738daa8b4b4a
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60947338"
---
# <a name="printtask-resource-type"></a>тип ресурса printTask

Пространство имен: microsoft.graph

Представляет задачу, выполненную или выполненную в результате события универсальной печати.

Дополнительные сведения о том, как использовать этот ресурс для добавления поддержки печати в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Список (от printTaskDefintion)](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | Получите список задач, созданных на основе определенного шрифтаTaskDefinition. Список включает в себя выполнение текущих задач и недавно завершенных задач. |
| [Получение](../api/printtask-get.md); | [printTask](printtask.md) | Сведения о задаче печати. |
| [Обновление](../api/printtaskdefinition-update-task.md) | [printTask](printtask.md) | Обновляет задачу печати. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор printTask. Только для чтения.|
|status|[printTaskStatus](printtaskstatus.md)|Текущее состояние выполнения этого printTask. **Приложение вызовов отвечает за обновление этого состояния по завершению обработки, если соответствующий printJob не был перенаправлен на другой принтер.** Невыполнение отчетов о завершении приведет к блокировке связанного задания печати от печати и в конечном итоге к их удаляемой работе. |
|parentUrl|String|URL-адрес для объекта печати, который вызвал эту задачу. Например, `https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{jobId}`. Только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|триггер|[printTaskTrigger](printtasktrigger.md)|PrintTaskTrigger, который вызвал выполнение этой задачи. Только для чтения.|
|определение|[printTaskDefinition](printtaskdefinition.md)|PrintTaskDefinition, который использовался для создания этой задачи. Только для чтения.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printTask",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTask",
  "id": "String (identifier)",
  "status": {
    "@odata.type": "microsoft.graph.printTaskStatus"
  },
  "parentUrl": "String"
}
```

