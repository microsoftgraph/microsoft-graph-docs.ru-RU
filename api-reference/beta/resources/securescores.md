---
title: Тип ресурса secureScores
description: 'в начало = n, где n — число дней данных, которую необходимо получить. '
localization_priority: Normal
ms.openlocfilehash: 8b4be9822b782303efe38dbdf5bd43e1ee543421
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640184"
---
# <a name="securescores-resource-type"></a>Тип ресурса secureScores

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет безопасной счета клиента в день для оценки данных, на уровне клиента и элемента управления. По умолчанию проводится данных в течение 90 дней. Эти данные сортируются по **createdDateTime**от поздних к ранним. Это позволит вам для запросов с помощью $top = n, где n — число дней данных, которую необходимо получить. 


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Перечисление объектов secureScores](../api/securescores-list.md) | [secureScores](securescores.md) |Чтение свойства и метаданные объекта secureScores.|


## <a name="properties"></a>Свойства
Свойства содержащий тип сущности безопасности клиента широкополосном (ежедневного моментальный снимок данных).

|Свойство |Тип |Описание |
|:--|:--|:--|
|   azureTenantId   |   String  |   Идентификатор GUID строки для клиента.  |
|   createdDateTime |   DateTimeOffset  |   Дата создания объекта.  |
|   id  |   String  |   Сочетание azureTenantId_createdDateTime.   |
|   licensedUserCount   |   Int32   |   Число пользователей данного клиента с корпоративным лицензированием.    |
|   activeUserCount |   Int32   |   Число активных пользователей указанного клиента.  |
|   currentScore    |   Double  |   Оценка текущего обновления клиента на указанной даты.    |
|   maxScore |  Double  |   Клиент максимальное возможному значению на указанной даты.    |
|   enabledServices |   Коллекция String   |   Службы Майкрософт для клиента (например, Exchange online, Скайп, Sharepoint).   |
|   averageComparativeScores |  [averageComparativeScore](averagecomparativescore.md) коллекции    |Средняя оценка по различные области (например, среднее число разных отраслей, среднее, число) и элемент управления категории (удостоверения, данные, устройства, приложения, инфраструктуры) в области действия. |
|   controlScores | [controlScore](controlscore.md) коллекции  |   Содержит показателям клиента для набора элементов управления.   |


## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
}-->

```json
{
"id": "String",
"azureTenantId": "Guid",
"createdDate": "DateTimeOffset",
"licensedUserCount": "Int32",
"activeUserCount": "Int32",
"currentScore": "Int32",
"maxScore": "Int32",
"averageScore": "Double",
"enabledServices": "Collection(string)",
"averageComparativeScores": "Collection(microsoft.graph.SecureScore.averageComparativeScores)",
"controlScores": "Collection(microsoft.graph.SecureScore.controlScores)",
}

```


<!--
{
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescores.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
