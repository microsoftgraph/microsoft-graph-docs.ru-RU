---
title: тип ресурса teamsAsyncOperation
description: 'Операция Microsoft Teams async — это операция, которая выходит за рамки срока службы одного запроса API. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2db0708ada9bb57ad4f0f88da89c797ff4a4e1e2
ms.sourcegitcommit: 596b3d5636f3f3e042d180ea8f039f00ebd6b38a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2021
ms.locfileid: "53665902"
---
# <a name="teamsasyncoperation-resource-type"></a>тип ресурса teamsAsyncOperation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Операция Microsoft Teams async — это операция, которая выходит за рамки срока службы одного запроса API. Эти операции являются длительными или слишком дорогими для выполнения в период времени, зарожаемого запросом.

При инициировании операции async метод возвращает код ответа 202 Accepted. В ответе также будет содержаться загон расположения, который содержит расположение teamsAsyncOperation. Периодически проверяйте состояние операции, делая запрос GET в этом расположении; подождите >30 секунд между проверками.
После успешного завершения запроса состояние будет "успешным", а целевое значениеResourceLocation будет указать на созданный или измененный ресурс.

## <a name="methods"></a>Методы

|  Метод                                                                   |  Возвращаемый тип                                                                     | Описание                                                       | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :---------------------------------------------------------------- |
| [Список операций в чате](../api/chat-list-operations.md)               | Коллекция [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Список операций async, которые запускались или запускались в определенном чате. |
| [Получить операцию](../api/teamsasyncoperation-get.md)                   | Коллекция [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Получите операцию async, которая запущена или запущена на определенном ресурсе. |

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание |
|:---------------|:--------|:----------|
|id|строка |Уникальный id операции.|
|operationType|[teamsAsyncOperationType](teamsasyncoperationtype.md) |Обозначает тип описываемой операции. |
|createdDateTime|DateTimeOffset |Время создания операции.|
|status|[teamsAsyncOperationStatus](teamsasyncoperationstatus.md)| Состояние операции.|
|lastActionDateTime|DateTimeOffset |Время последнего обновления операции async.|
|attemptsCount|Int32|Количество попыток операции, прежде чем она была отмечена успешной или неудачной.|
|targetResourceId|guid |ID объекта, созданного или измененного в результате этой операции async, как правило, [группы](../resources/team.md).|
|targetResourceLocation|строка|Расположение объекта, созданного или измененного в результате этой операции async. Этот URL-адрес должен рассматриваться как непрозрачная величина, а не разрезать его пути компонентов.|
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
    "operationType": "string",
    "createdDateTime": "string (timestamp)",
    "status": "string",
    "lastActionDateTime": "string (timestamp)",
    "attemptsCount": "Integer",
    "targetResourceId": "string",
    "targetResourceLocation": "string",
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
  "suppressions": []
}
-->


