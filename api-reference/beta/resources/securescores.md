---
title: Тип ресурса secureScores
description: 'в начало = n, где n — число дней данных, которую необходимо получить. '
localization_priority: Normal
ms.openlocfilehash: fef5c43130aecf1604677d07f785a0cee0539568
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576082"
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
|   azureTenantId   |   Строка  |   Идентификатор GUID строки для клиента.  |
|   createdDateTime |   DateTimeOffset  |   Дата создания объекта.  |
|   id  |   Строка  |   Сочетание azureTenantId_createdDateTime.   |
|   licensedUserCount   |   Int32   |   Число пользователей данного клиента с корпоративным лицензированием.    |
|   activeUserCount |   Int32   |   Число активных пользователей указанного клиента.  |
|   currentScore    |   Double  |   Оценка текущего обновления клиента на указанной даты.    |
|   maxScore |  Double  |   Клиент максимальное возможному значению на указанной даты.    |
|   enabledServices |   Коллекция String   |   Службы Майкрософт для клиента (например, Exchange online, Скайп, Sharepoint).   |
|   averageComparativeScores |  [averageComparativeScore](averagecomparativescore.md) коллекции    |Средняя оценка по различные области (например, среднее число разных отраслей, среднее, число) и элемент управления категории (удостоверения, данные, устройства, приложения, инфраструктуры) в области действия. |
|   controlScores | [controlScore](controlscore.md) коллекции  |   Содержит показателям клиента для набора элементов управления.   |
|   vendorInformation | [securityVendorInformation](securityvendorinformation.md) | Содержит сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = корпорации Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker).|

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
    "azureTenantId": "String (identifier)",
    "createdDateTime": "DateTimeOffset",
    "licensedUserCount": "Int32",
    "activeUserCount": "Int32",
    "currentScore": "Double",
    "maxScore": "Double",    
    "enabledServices": ["String"],
    "averageComparativeScores": [{ "@odata.type":"microsoft.graph.averageComparativeScores"}],
    "controlScores": [{"@odata.type":"microsoft.graph.controlScores"}],
    "vendorInformation" : "microsoft.graph.securityVendorInformation"
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
