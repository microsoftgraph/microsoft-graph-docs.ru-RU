---
title: Тип ресурса printJob
description: Представляет задание печати, помещенное в очередь для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5eff75fba2c9993275c277877fedec7705021c49
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896005"
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
| [Начало](../api/printjob-startprintjob.md)|Нет|Запустите задание печати.|
| [Отмена](../api/printjob-cancelprintjob.md)|Нет|Отмена задания печати.|

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