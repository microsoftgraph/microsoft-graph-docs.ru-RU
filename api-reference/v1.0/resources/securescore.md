---
title: тип ресурса secureScore
description: Представляет безопасную оценку клиента в день подсчета данных на уровне клиента и управления.
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 01499bbd755739310bc309656379bde278401544
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084127"
---
# <a name="securescore-resource-type"></a>тип ресурса secureScore

Пространство имен: microsoft.graph

Представляет безопасную оценку клиента в день подсчета данных на уровне клиента и управления. По умолчанию проводится 90 дней хранения данных. Эти данные сортируют **по createdDateTime**, от последней до ранней. Это позволит вам страница ответы с помощью $top=n, где n = количество дней данных, которые вы хотите получить. 


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Перечисление объектов secureScores](../api/security-list-securescores.md) | [коллекция secureScores](securescore.md) |Получите коллекцию объектов secureScore.|
|[Получение объектов secureScore](../api/securescore-get.md) | [secureScore](securescore.md) |Чтение свойств и метаданных объекта secureScore. | 



## <a name="properties"></a>Свойства

|Свойство |Тип |Описание |
|:--|:--|:--|
|id |String|GUID или уникальный идентификатор, созданный поставщиком. Только для чтения. Обязательный.|
|   azureTenantId   |   String  |   Строка GUID для ID клиента.  |
|   activeUserCount |   Int32   |   Активный учет пользователей данного клиента.  |
|   createdDateTime |   DateTimeOffset  |   Дата создания объекта.  |
|   currentScore    |   Двойное с плавающей точкой  |   Текущая оценка клиента в указанную дату.    |
|   enabledServices |   Коллекция String   |   Службы, предоставляемые Корпорацией Майкрософт для клиента (например, Exchange, Skype, Sharepoint).   |
|   licensedUserCount   |   Int32   |   Количество лицензированных пользователей данного клиента.    |
|   maxScore |  Двойное с плавающей точкой  |   Максимально возможный балл клиента в указанную дату.    |
|   averageComparativeScores |  [коллекция averageComparativeScore](averagecomparativescore.md)    |Средняя оценка по различным сферам (например, в среднем по отрасли, в среднем по местам) и категории управления (Identity, Data, Device, Apps, Infrastructure) в пределах области. |
|   controlScores | [коллекция controlScore](controlscore.md)  |   Содержит оценки клиента для набора элементов управления.   |
|vendorInformation |[securityVendorInformation](securityvendorinformation.md)|Сложный тип, содержащий сведения о поставщике продукта и службы безопасности, поставщике и подпрограмме (например, vendor=Microsoft; provider=SecureScore). Обязательный.|


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

