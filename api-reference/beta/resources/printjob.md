---
title: тип ресурса printJob
description: Представляет задание печати, которое выстроилось в очередь для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 170f413c7607933c2651720c9c9c463f90cf55df
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516530"
---
# <a name="printjob-resource-type"></a>тип ресурса printJob

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет задание печати, которое выстроилось в очередь для принтера.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [получение](../api/printjob-get.md); | [printJob](printjob.md) | Чтение свойств и связей объекта printJob. |
| [Создание](../api/printer-post-jobs.md) | [printJob](printjob.md) | Создание нового объекта задания печати. |
| [обновление](../api/printjob-update.md). | [printJob](printjob.md) | Обновление объекта задания печати. |
| [Начало](../api/printjob-start.md)|Нет|Запустите задание печати.|
| [Отмена](../api/printjob-cancel.md)|Нет|Отмена задания печати.|
| [Прервать](../api/printjob-abort.md)|Нет|Прервать задание печати.|
| [Перенаправление (на другой принтер)](../api/printjob-redirect.md) | [printJob](printjob.md) | Задание печати, которое находится в очереди для принтера назначения. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|GUID принтера. Только для чтения.|
|createdDateTime|DateTimeOffset|DateTimeOffset, когда задание было создано. Только для чтения.|
|status|[printJobStatus](printjobstatus.md)|Состояние задания печати. Только для чтения.|
|configuration|[printJobConfiguration](printJobConfiguration.md)|Группа параметров, которые принтер должен использовать для печати задания.|
|isFetchable|Edm.Boolean|Если это так, документ можно получить на принтере.|
|redirectedFrom|Edm.String|Содержит URL-адрес задания источника, если задание было перенаправлено с другого принтера.|
|redirectedTo|Edm.String|Содержит URL-адрес задания назначения, если задание было перенаправлено на другой принтер.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|createdBy|[userIdentity](useridentity.md)| Только для чтения. Допускается значение null.|
|документы|[коллекция printDocument](printdocument.md)| Только для чтения.|
|tasks|[printTask](printtask.md) collection|Список [printTasks,](printtask.md) которые были вызваны этим заданием печати.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJob",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "isFetchable": "Boolean",
  "redirectedFrom": "String",
  "redirectedTo": "String",
  "status": {"@odata.type": "microsoft.graph.printJobStatus"},
  "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
  "configuration": {"@odata.type": "microsoft.graph.printJobConfiguration"},
  "documents": [ {"@odata.type": "microsoft.graph.printDocument"} ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

