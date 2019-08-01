---
title: Тип ресурса Секурескоре
description: Представляет безопасное значение клиента в день данных оценки на уровне клиента и элемента управления.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 395c5ed0594d1f509bb664b5aee6ea18bb42af0a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034484"
---
# <a name="securescore-resource-type"></a>Тип ресурса Секурескоре

Представляет безопасное значение клиента в день данных оценки на уровне клиента и элемента управления. По умолчанию данные хранятся в 90 дней. Эти данные сортируются по **createdDateTime**, от последних к ранним. Это позволит получать ответы на страницы с помощью $top = n, где n = число дней, которые требуется получить. 


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Список объектов secureScore](../api/security-list-securescores.md) | Коллекция [секурескорес](securescore.md) |Получение коллекции объектов Секурескоре.|
|[Получение объектов secureScore](../api/securescore-get.md) | [Секурескоре](securescore.md) |Чтение свойств и метаданных объекта Секурескоре. | 



## <a name="properties"></a>Свойства

|Свойство |Тип |Описание |
|:--|:--|:--|
|id |String|GUID или уникальный идентификатор, созданный поставщиком. Только для чтения. Обязательный атрибут.|
|   azureTenantId   |   String  |   Строка GUID для идентификатора клиента.  |
|   Активеусеркаунт |   Int32   |   Число активных пользователей для данного клиента.  |
|   createdDateTime |   DateTimeOffset  |   Дата создания объекта.  |
|   Куррентскоре    |   Двойное  |   Текущий полученный рейтинг клиента на указанную дату.    |
|   Енабледсервицес |   Коллекция строк   |   Службы, предоставляемые корпорацией Майкрософт для клиента (например, Exchange Online, Skype, SharePoint).   |
|   Лиценседусеркаунт   |   Int32   |   Число лицензированных пользователей для данного клиента.    |
|   Максскоре |  Двойное  |   Максимальная возможная Оценка клиента на указанную дату.    |
|   Аверажекомпаративескорес |  Коллекция [аверажекомпаративескоре](averagecomparativescore.md)    |Средняя оценка по различным областям (например, усреднение по отраслям, среднему на количество участников) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура) в области. |
|   Контролскорес | Коллекция [контролскоре](controlscore.md)  |   Содержит результаты клиентов для набора элементов управления.   |
|vendorInformation |[securityVendorInformation](securityvendorinformation.md)|Сложный тип, содержащий сведения о продукте, поставщике, поставщике и подобеспечении безопасности (например, Vendor = Microsoft; Provider = Секурескоре). Обязательно.|


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
"id": "String (identifier)",
"azureTenantId": "String",
"activeUserCount": "Int32",
"createdDateTime": "String (timestamp)",
"currentScore": "Double",
"enabledServices": ["String"],
"licensedUserCount": "Int32",
"maxScore": "Double",
"averageComparativeScores": [{"@odata.type": "microsoft.graph.averageComparativeScore"}],
"controlScores": [{"@odata.type": "microsoft.graph.controlScore"}],
"vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "secureScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
