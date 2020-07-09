---
title: Тип ресурса printJob
description: Представляет задание печати, помещенное в очередь для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 0d46263e5f393362cec155a9be3e2e5a54c3dfec
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091524"
---
# <a name="printjob-resource-type"></a>Тип ресурса printJob

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет задание печати, помещенное в очередь для принтера.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [получение](../api/printjob-get.md); | [printJob](printjob.md) | Чтение свойств и связей объекта printJob. |
| [Создание](../api/printer-post-jobs.md); | [printJob](printjob.md) | Создание нового объекта задания печати. |
| [Начало](../api/printjob-startprintjob.md)|Отсутствует|Запустите задание печати.|
| [Отмена](../api/printjob-cancelprintjob.md)|Отсутствует|Отмена задания печати.|
| [Перенаправление (на другой принтер)](../api/printjob-redirect.md) | [printJob](printjob.md) | Задание печати, помещенное в очередь для конечного принтера. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|GUID принтера. Только для чтения.|
|createdDateTime|DateTimeOffset|Значение DateTimeOffset при создании задания. Только для чтения.|
|status|[принтжобстатус](printjobstatus.md)|Состояние задания печати. Только для чтения.|

## <a name="relationships"></a>Отношения
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|createdBy|[userIdentity](useridentity.md)| Только для чтения. Допускается значение null.|
|настоящему|Коллекция [printDocument](printdocument.md)| Только для чтения.|
|tasks|Коллекция [принттаск](printtask.md)|Список [принттаскс](printtask.md) , которые были активированы этим заданием печати.|

## <a name="json-representation"></a>Представление в формате JSON

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
  "status": {"@odata.type": "microsoft.graph.printJobStatus"},
  "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
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