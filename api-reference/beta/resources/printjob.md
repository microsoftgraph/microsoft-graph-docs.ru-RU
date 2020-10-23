---
title: Тип ресурса printJob
description: Представляет задание печати, помещенное в очередь для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7810c8cd864020c42de4482deea67620950f6cf0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726306"
---
# <a name="printjob-resource-type"></a>Тип ресурса printJob

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет задание печати, помещенное в очередь для принтера.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [получение](../api/printjob-get.md); | [printJob](printjob.md) | Чтение свойств и связей объекта printJob. |
| [создание](../api/printer-post-jobs.md); | [printJob](printjob.md) | Создание нового объекта задания печати. |
| [Начало](../api/printjob-start.md)|Нет|Запустите задание печати.|
| [Отмена](../api/printjob-cancel.md)|Нет|Отмена задания печати.|
| [Перенаправление (на другой принтер)](../api/printjob-redirect.md) | [printJob](printjob.md) | Задание печати, помещенное в очередь для конечного принтера. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка|GUID принтера. Только для чтения.|
|createdDateTime|DateTimeOffset|Значение DateTimeOffset при создании задания. Только для чтения.|
|status|[принтжобстатус](printjobstatus.md)|Состояние задания печати. Только для чтения.|
|configuration|[принтжобконфигуратион](printJobConfiguration.md)|Группа параметров, которые принтер должен использовать для печати задания.|
|подбираемый|Edm.Boolean|Если этот параметр имеет значение true, документ может быть извлечен принтером.|
|редиректедфром|Edm.String|Содержит URL-адрес исходного задания, если задание было перенаправлено с другого принтера.|
|редиректедто|Edm.String|Содержит URL-адрес конечного задания, если задание было перенаправлено на другой принтер.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|createdBy|[userIdentity](useridentity.md)| Только для чтения. Допускается значение null.|
|настоящему|Коллекция [printDocument](printdocument.md)| Только для чтения.|
|tasks|Коллекция [принттаск](printtask.md)|Список [принттаскс](printtask.md) , которые были активированы этим заданием печати.|

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

