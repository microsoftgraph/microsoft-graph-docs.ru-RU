---
title: Тип ресурса secureScores
description: 'в начало = n, где n — число дней данных, которую необходимо получить. '
ms.openlocfilehash: 96d5c487bb854559b0128d93ea8e0783fcc61f0c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075650"
---
# <a name="securescores-resource-type"></a>Тип ресурса secureScores

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет безопасной счета клиента в день для оценки данных, на уровне клиента и элемента управления. По умолчанию проводится данных в течение 90 дней. Эти данные сортируются по **createdDateTime**от поздних к ранним. Это позволит вам для запросов с помощью $top = n, где n — число дней данных, которую необходимо получить. 


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Список secureScores](../api/securescores-list.md) | [secureScores](securescores.md) |Чтение свойства и метаданные объекта secureScores.|


## <a name="properties"></a>Свойства
Свойства содержащий тип сущности безопасности клиента широкополосном (ежедневного моментальный снимок данных).

|Свойство |Тип |Description |
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


<!-- {
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
