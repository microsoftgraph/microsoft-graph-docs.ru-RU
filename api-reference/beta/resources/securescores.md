---
title: Тип ресурса Секурескоре
description: 'TOP = n, где n — это количество дней, в течение которых требуется получить данные. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 3db31203f9c5827459ab2149efbd3adb28030d0a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087546"
---
# <a name="securescore-resource-type"></a>Тип ресурса Секурескоре

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет безопасное значение клиента в день данных оценки на уровне клиента и элемента управления. По умолчанию данные хранятся в 90 дней. Эти данные сортируются по **createdDateTime**, от последних к ранним. Это позволит получать ответы на страницы с помощью $top = n, где n = число дней, которые требуется получить.


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Список объектов secureScore](../api/securescores-list.md) | [secureScores](securescores.md) |Чтение свойств и метаданных объекта Секурескорес.|


## <a name="properties"></a>Свойства
Тип объекта, содержащий свойства оценки безопасности клиента (ежедневные данные моментального снимка).

|Свойство |Тип |Описание |
|:--|:--|:--|
|   azureTenantId   |   String  |   Строка GUID для идентификатора клиента.  |
|   createdDateTime |   DateTimeOffset  |   Дата создания объекта.  |
|   id  |   Строка  |   Сочетание azureTenantId_createdDateTime.   |
|   лиценседусеркаунт   |   Int32   |   Число лицензированных пользователей для данного клиента.    |
|   активеусеркаунт |   Int32   |   Число активных пользователей для данного клиента.  |
|   куррентскоре    |   Двойное с плавающей точкой  |   Текущий полученный рейтинг клиента на указанную дату.    |
|   максскоре |  Двойное с плавающей точкой  |   Максимальная возможная Оценка клиента на указанную дату.    |
|   енабледсервицес |   Коллекция String   |   Службы, предоставляемые корпорацией Майкрософт для клиента (например, Exchange Online, Skype, SharePoint).   |
|   аверажекомпаративескорес |  Коллекция [аверажекомпаративескоре](averagecomparativescore.md)    |Средняя оценка по различным областям (например, усреднение по отраслям, среднему на количество участников) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура) в области. |
|   контролскорес | Коллекция [контролскоре](controlscore.md)  |   Содержит результаты клиентов для набора элементов управления.   |


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


