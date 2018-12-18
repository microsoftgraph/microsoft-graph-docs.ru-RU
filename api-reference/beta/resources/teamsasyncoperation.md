---
title: Тип ресурса teamsAsyncOperation
description: 'Операцию асинхронного группами Майкрософт — это операция, выходит за рамки жизненным циклом одним запросом API. '
author: nkramer
ms.openlocfilehash: f88f5eba32fbd0629bf66a61dca963a7815988fd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305560"
---
# <a name="teamsasyncoperation-resource-type"></a>Тип ресурса teamsAsyncOperation

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Операцию асинхронного группами Майкрософт — это операция, выходит за рамки жизненным циклом одним запросом API. Эти операции выполняются длительным или слишком дорого для выполнения в рамках интервала времени их исходного запроса.

При запуске асинхронной операции, метод возвращает 202 код ответа принято. Ответ также будет содержать заголовок расположения, который содержит расположение teamsAsyncOperation. Периодически проверяйте состояние операции, сделав запрос GET по этому адресу; Подождите > 30 секунд между проверок.
После успешного завершения запроса состояния будет иметь «выполнена успешно» и targetResourceLocation будет указывать на ресурс созданные или измененные.

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание |
|:---------------|:--------|:----------|
|id|строка |Операция уникальный идентификатор.|
|operationType|[teamsAsyncOperationType](teamsasyncoperationtype.md) |Указывает, какой тип операции, описанного.|
|createdDateTime|DateTimeOffset |Время создания операции.|
|status|[teamsAsyncOperationStatus](teamsasyncoperationstatus.md)| Состояние операции.|
|lastActionDateTime|DateTimeOffset |Время последнего обновления асинхронной операции.|
|attemptsCount|Int32|Количество раз, когда операция перед помечаются как успешные и неудачные.|
|targetResourceId|Идентификатор GUID |Идентификатор объекта, который создал или изменены в результате этой асинхронной операции, обычно [группы](../resources/team.md).|
|targetResourceLocation|string|Расположение объекта, который создал или изменил как результат этой асинхронной операции. Этот URL-адрес следует рассматривать как Непрозрачное значение и не синтаксический анализ в его компонента пути.|
|error|[operationError](operationerror.md)|Любая ошибка, которая приводит к сбою асинхронной операции.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsasyncoperation"
}-->

```json
{
    "id": "string",
    "operationType": "archiveTeam",
    "createdDateTime": "2018-01-01T00:00:00.0000000Z",
    "status": "succeeded",
    "lastActionDateTime": "2018-01-01T00:00:00.0000000Z",
    "attemptsCount": 1,
    "targetResourceId": "fa4aa5a2-a75b-4769-86f4-9e2742a18fda",
    "targetResourceLocation": "/groups('fa4aa5a2-a75b-4769-86f4-9e2742a18fda')/team",
    "error": null
}
```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
