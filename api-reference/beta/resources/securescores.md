---
title: Тип ресурса secureScore
description: 'top=n, где n = количество дней данных, которые требуется получить. '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: 9565a507eac6d5c1be272749a45c6e4b234d5da2
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094097"
---
# <a name="securescore-resource-type"></a>Тип ресурса secureScore

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет оценку безопасности клиента за день оценки данных на уровне клиента и управления. По умолчанию данные хранятся в течение 90 дней. Эти данные сортируются по **параметру createdDateTime** от последней до ранней версии. Это позволит отображать ответы на страницы с помощью $top=n, где n = количество дней данных, которые требуется извлечь.


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Перечисление объектов secureScores](../api/securescores-list.md) | [secureScores](securescores.md) |Чтение свойств и метаданных объекта secureScores.|


## <a name="properties"></a>Свойства
Тип сущности, содержащий свойства оценки безопасности клиента (данные ежедневных моментальных снимков).

|Свойство |Тип |Описание |
|:--|:--|:--|
|   activeUserCount |   Int32   |   Число активных пользователей заданного клиента.  |
|   averageComparativeScores |  [Коллекция averageComparativeScore](averagecomparativescore.md)    |Средняя оценка по различным областям (например, среднее по отрасли, среднее по рабочим местам) и категории элементов управления (удостоверение, данные, устройство, приложения, инфраструктура) в этой области. |
|   azureTenantId   |   String  |   Строка GUID для идентификатора клиента.  |
|   controlScores | [Коллекция controlScore](controlscore.md)  |   Содержит оценки клиентов для набора элементов управления.   |
|   createdDateTime |   DateTimeOffset  |   Дата создания сущности.  |
|   currentScore    |   Двойное с плавающей точкой  |   Текущая оценка клиента за указанную дату.    |
|   enabledServices |   Коллекция String   |   Предоставляемые корпорацией Майкрософт службы для клиента (например, Exchange online, Skype, SharePoint).   |
|   id  |   String  |   Сочетание azureTenantId_createdDateTime.   |
|   licensedUserCount   |   Int32   |   Число лицензированных пользователей заданного клиента.    |
|   maxScore |  Двойное с плавающей точкой  |   Максимально возможная оценка клиента в указанную дату.    |




## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScore"
}-->

```json
{
  "activeUserCount": "Int32",
  "averageComparativeScores": "Collection(microsoft.graph.SecureScore.averageComparativeScores)",
  "averageScore": "Double",
  "azureTenantId": "Guid",
  "controlScores": "Collection(microsoft.graph.SecureScore.controlScores)",
  "createdDate": "DateTimeOffset",
  "createdDateTime": "2019-02-07T20:33:53.156Z",
  "currentScore": "Int32",
  "enabledServices": "Collection(string)",
  "id": "String",
  "licensedUserCount": "Int32",
  "maxScore": "Int32"
}
```


<!--
{
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


