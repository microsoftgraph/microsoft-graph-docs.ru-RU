---
title: Тип ресурса Секурескорес
description: 'TOP = n, где n — это количество дней, в течение которых требуется получить данные. '
localization_priority: Normal
ms.openlocfilehash: 8b4be9822b782303efe38dbdf5bd43e1ee543421
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549211"
---
# <a name="securescores-resource-type"></a>Тип ресурса Секурескорес

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет безопасное значение клиента в день данных оценки на уровне клиента и элемента управления. По умолчанию данные хранятся в 90 дней. Эти данные сортируются по **createdDateTime**, от последних к ранним. Это позволит получать ответы на страницы с помощью $top = n, где n = число дней, которые требуется получить. 


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Перечисление объектов secureScores](../api/securescores-list.md) | [Секурескорес](securescores.md) |Чтение свойств и метаданных объекта Секурескорес.|


## <a name="properties"></a>Свойства
Тип объекта, содержащий свойства оценки безопасности клиента (ежедневные данные моментального снимка).

|Свойство |Тип |Описание |
|:--|:--|:--|
|   Азуретенантид   |   String  |   Строка GUID для идентификатора клиента.  |
|   createdDateTime |   DateTimeOffset  |   Дата создания объекта.  |
|   id  |   String  |   Сочетание Азуретенантид_креатеддатетиме.   |
|   Лиценседусеркаунт   |   Int32   |   Число лицензированных пользователей для данного клиента.    |
|   Активеусеркаунт |   Int32   |   Число активных пользователей для данного клиента.  |
|   Куррентскоре    |   Двойное  |   Текущий полученный рейтинг клиента на указанную дату.    |
|   Максскоре |  Двойное  |   Максимальная возможная Оценка клиента на указанную дату.    |
|   Енабледсервицес |   Коллекция строк   |   Службы, предоставляемые корпорацией Майкрософт для клиента (например, Exchange Online, Skype, SharePoint).   |
|   Аверажекомпаративескорес |  Коллекция [аверажекомпаративескоре](averagecomparativescore.md)    |Средняя оценка по различным областям (например, усреднение по отраслям, среднему на количество участников) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура) в области. |
|   Контролскорес | Коллекция [контролскоре](controlscore.md)  |   Содержит результаты клиентов для набора элементов управления.   |


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
