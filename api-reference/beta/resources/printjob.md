---
title: Тип ресурса printJob
description: Представляет задание печати, которое было в очереди для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 43b08c39715c9984a1692c0bcb823881be4ab4d1
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784831"
---
# <a name="printjob-resource-type"></a>Тип ресурса printJob

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет задание печати, которое было в очереди для принтера.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [получение](../api/printjob-get.md); | [printJob](printjob.md) | Чтение свойств и связей объекта printJob. |
| [Создание](../api/printer-post-jobs.md) | [printJob](printjob.md) | Создание объекта задания печати. |
| [Начало](../api/printjob-start.md)|Нет|Запустите задание печати.|
| [Отмена](../api/printjob-cancel.md)|Нет|Отмените задание печати.|
| [Прервать](../api/printjob-abort.md)|Нет|Отменить задание печати.|
| [Перенаправление (на другой принтер)](../api/printjob-redirect.md) | [printJob](printjob.md) | Задание печати, которое находится в очереди для принтера назначения. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|GUID принтера. Только для чтения.|
|createdDateTime|DateTimeOffset|DateTimeOffset, когда было создано задание. Только для чтения.|
|status|[printJobStatus](printjobstatus.md)|Состояние задания печати. Только для чтения.|
|configuration|[printJobConfiguration](printJobConfiguration.md)|Группа параметров, которые принтер должен использовать для печати задания.|
|isFetchable|Edm.Boolean|Если засвеяно, документ может быть извлечен принтером.|
|redirectedFrom|Edm.String|Содержит URL-адрес задания источника, если задание было перенаправлено с другого принтера.|
|redirectedTo|Edm.String|Содержит URL-адрес задания назначения, если задание было перенаправлено на другой принтер.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|createdBy|[userIdentity](useridentity.md)| Только для чтения. Допускается значение null.|
|documents|[Коллекция printDocument](printdocument.md)| Только для чтения.|
|tasks|[Коллекция printTask](printtask.md)|Список [printTasks,](printtask.md) которые были инициированы этим заданием печати.|

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

