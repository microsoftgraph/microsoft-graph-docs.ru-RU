---
title: Тип ресурса secureScore
description: 'top=n, где n = количество дней данных, которые требуется получить. '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: f289ef7c91dbe7975970e679d1950a03498ab333
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900130"
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
|   azureTenantId   |   String  |   Строка GUID для идентификатора клиента.  |
|   createdDateTime |   DateTimeOffset  |   Дата создания сущности.  |
|   id  |   Строка  |   Сочетание azureTenantId_createdDateTime.   |
|   licensedUserCount   |   Int32   |   Число лицензированных пользователей заданного клиента.    |
|   activeUserCount |   Int32   |   Число активных пользователей заданного клиента.  |
|   currentScore    |   Двойное с плавающей точкой  |   Текущая оценка клиента за указанную дату.    |
|   maxScore |  Двойное с плавающей точкой  |   Максимально возможная оценка клиента в указанную дату.    |
|   enabledServices |   Коллекция String   |   Предоставляемые корпорацией Майкрософт службы для клиента (например, Exchange Online, Skype, Sharepoint).   |
|   averageComparativeScores |  [Коллекция averageComparativeScore](averagecomparativescore.md)    |Средняя оценка по различным областям (например, среднее по отрасли, среднее по рабочим местам) и категории элементов управления (удостоверение, данные, устройство, приложения, инфраструктура) в этой области. |
|   controlScores | [Коллекция controlScore](controlscore.md)  |   Содержит оценки клиентов для набора элементов управления.   |


## <a name="relationships"></a>Отношения

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
  "createdDateTime": "2019-02-07T20:33:53.156Z"
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


