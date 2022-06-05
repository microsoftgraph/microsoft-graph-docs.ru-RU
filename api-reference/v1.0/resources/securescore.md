---
title: Тип ресурса secureScore
description: Представляет оценку безопасности клиента за день оценки данных на уровне клиента и управления.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 4773436fa1ef3f2e2465b99cd9c29e2d844d8b54
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900389"
---
# <a name="securescore-resource-type"></a>Тип ресурса secureScore

Пространство имен: microsoft.graph

Представляет оценку безопасности клиента за день оценки данных на уровне клиента и управления. По умолчанию данные хранятся в течение 90 дней. Эти данные сортируются по **параметру createdDateTime** от последней до ранней версии. Это позволит отображать ответы на страницы с помощью $top=n, где n = количество дней данных, которые требуется извлечь. 


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Перечисление объектов secureScores](../api/security-list-securescores.md) | [Коллекция secureScores](securescore.md) |Получение коллекции объектов secureScore.|
|[Получение объектов secureScore](../api/securescore-get.md) | [secureScore](securescore.md) |Чтение свойств и метаданных объекта secureScore. | 



## <a name="properties"></a>Свойства

|Свойство |Тип |Описание |
|:--|:--|:--|
|id |String|GUID или уникальный идентификатор, созданный поставщиком. Только для чтения. Обязательный.|
|   azureTenantId   |   String  |   Строка GUID для идентификатора клиента.  |
|   activeUserCount |   Int32   |   Число активных пользователей заданного клиента.  |
|   createdDateTime |   DateTimeOffset  |   Дата создания сущности.  |
|   currentScore    |   Двойное с плавающей точкой  |   Текущая оценка клиента за указанную дату.    |
|   enabledServices |   Коллекция String   |   Предоставляемые корпорацией Майкрософт службы для клиента (например, Exchange Online, Skype, Sharepoint).   |
|   licensedUserCount   |   Int32   |   Число лицензированных пользователей заданного клиента.    |
|   maxScore |  Двойное с плавающей точкой  |   Максимально возможная оценка клиента в указанную дату.    |
|   averageComparativeScores |  [Коллекция averageComparativeScore](averagecomparativescore.md)    |Средняя оценка по различным областям (например, среднее по отрасли, среднее по рабочим местам) и категории элементов управления (удостоверение, данные, устройство, приложения, инфраструктура) в этой области. |
|   controlScores | [Коллекция controlScore](controlscore.md)  |   Содержит оценки клиентов для набора элементов управления.   |
|vendorInformation |[securityVendorInformation](securityvendorinformation.md)|Сложный тип, содержащий сведения о поставщике продукта или службы безопасности, поставщике и субпроидере (например, vendor=Microsoft; provider=SecureScore). Обязательный.|


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

