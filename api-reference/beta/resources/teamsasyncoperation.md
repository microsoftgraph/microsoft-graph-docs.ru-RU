---
title: Тип ресурса Теамсасинкоператион
description: 'Асинхронная операция Microsoft Teams — это операция, не истечение срока действия одного запроса API. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c016b90ae6198204e9b99e3ae1e8d72b22919e8b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345772"
---
# <a name="teamsasyncoperation-resource-type"></a>Тип ресурса Теамсасинкоператион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Асинхронная операция Microsoft Teams — это операция, не истечение срока действия одного запроса API. Эти операции долго выполняются или слишком дороги для завершения в течение периода действия исходного запроса.

При запуске асинхронной операции метод возвращает код ответа, принятый в 202. В ответе также будет содержаться заголовок Location, который содержит расположение Теамсасинкоператион. Периодически проверяйте состояние операции, выполнив запрос GET к этому расположению; Дождитесь >30 секунд между проверками.
После успешного выполнения запроса состояние будет "выполнено успешно", а Таржетресаурцелокатион будет указывать на ресурс "создано/изменено".

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание |
|:---------------|:--------|:----------|
|id|строка |Уникальный идентификатор операции.|
|Оператионтипе|[Объекта teamsasyncoperationtype](teamsasyncoperationtype.md) |Указывает, какие типы операций описаны.|
|createdDateTime|DateTimeOffset |Время создания операции.|
|status|[Теамсасинкоператионстатус](teamsasyncoperationstatus.md)| Состояние операции.|
|Ластактиондатетиме|DateTimeOffset |Время последнего обновления асинхронной операции.|
|Аттемптскаунт|Int32|Сколько раз была предпринята попытка выполнения операции до ее пометки как успешной или неудачной.|
|Таржетресаурцеид|кодом |Идентификатор объекта, созданного или измененного в результате асинхронной операции, как правило, [команды](../resources/team.md).|
|Таржетресаурцелокатион|строка|Расположение объекта, созданного или измененного в результате асинхронной операции. Этот URL-адрес должен считаться непрозрачным значением и не был проанализирован в пути к его компонентам.|
|error|[Оператионеррор](operationerror.md)|Любая ошибка, которая приводит к сбою асинхронной операции.|

## <a name="json-representation"></a>Представление в формате JSON

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
