---
title: Тип ресурса teamsAsyncOperation
description: 'Операцию асинхронного группами Майкрософт — это операция, выходит за рамки жизненным циклом одним запросом API. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 61c26b0d594ccdbad8020557f60c6f6b23a83254
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513461"
---
# <a name="teamsasyncoperation-resource-type"></a>Тип ресурса teamsAsyncOperation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Операцию асинхронного группами Майкрософт — это операция, выходит за рамки жизненным циклом одним запросом API. Эти операции выполняются длительным или слишком дорого для выполнения в рамках интервала времени их исходного запроса.

При запуске асинхронной операции, метод возвращает 202 код ответа принято. Ответ также будет содержать заголовок расположения, который содержит расположение teamsAsyncOperation. Периодически проверяйте состояние операции, сделав запрос GET по этому адресу; Подождите >30 секунд между проверок.
После успешного завершения запроса состояния будет иметь «выполнена успешно» и targetResourceLocation будет указывать на ресурс созданные или измененные.

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание |
|:---------------|:--------|:----------|
|id|string |Операция уникальный идентификатор.|
|operationType|[teamsAsyncOperationType](teamsasyncoperationtype.md) |Указывает, какой тип операции, описанного.|
|createdDateTime|DateTimeOffset |Время создания операции.|
|status|[teamsAsyncOperationStatus](teamsasyncoperationstatus.md)| Состояние операции.|
|lastActionDateTime|DateTimeOffset |Время последнего обновления асинхронной операции.|
|attemptsCount|Int32|Количество раз, когда операция перед помечаются как успешные и неудачные.|
|targetResourceId|Guid |Идентификатор объекта, который создал или изменены в результате этой асинхронной операции, обычно [группы](../resources/team.md).|
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
<!--
{
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
