---
title: тип ресурса teamsAsyncOperation
description: 'Операция Microsoft Teams async выходит за пределы срока службы одного запроса API. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 643a7f57253af36e52484166492fd1e373f4ff5415ce24f1ccf84b69a3ec4fd1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196539"
---
# <a name="teamsasyncoperation-resource-type"></a>тип ресурса teamsAsyncOperation

Пространство имен: microsoft.graph



Операция Microsoft Teams async — это операция, которая выходит за рамки срока службы одного запроса API. Эти операции являются длительными или слишком дорогими для выполнения в период времени, зарожаемого запросом.

При инициировании операции async метод возвращает код ответа 202 Accepted. В ответе также будет содержаться загон расположения, который содержит расположение teamsAsyncOperation. Периодически проверяйте состояние операции, делая запрос GET в этом расположении; подождите >30 секунд между проверками.
После успешного завершения запроса состояние будет "успешным", а целевое значениеResourceLocation будет указать на созданный или измененный ресурс.

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание |
|:---------------|:--------|:----------|
|id|строка |Уникальный id операции.|
|operationType|[teamsAsyncOperationType](teamsasyncoperationtype.md) |Обозначает, какой тип операции описывается.|
|createdDateTime|DateTimeOffset |Время создания операции.|
|status|[teamsAsyncOperationStatus](teamsasyncoperationstatus.md)| Состояние операции.|
|lastActionDateTime|DateTimeOffset |Время последнего обновления операции async.|
|attemptsCount|Int32|Количество попыток операции, прежде чем она была отмечена успешной или неудачной.|
|targetResourceId|guid |ID объекта, созданного или измененного в результате этой операции async, как правило, [группы](../resources/team.md).|
|targetResourceLocation|Строка|Расположение объекта, созданного или измененного в результате этой операции async. Этот URL-адрес должен рассматриваться как непрозрачная величина, а не разрезать его пути компонентов.|
|error|[operationError](operationerror.md)|Любая ошибка, которая вызывает сбой операции async.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsAsyncOperation"
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

