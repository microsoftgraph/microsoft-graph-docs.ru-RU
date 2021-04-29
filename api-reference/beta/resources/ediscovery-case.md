---
title: тип ресурса case
description: В контексте eDiscovery содержатся хранители, хранитель, коллекции, наборы обзоров и экспорт.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 112a5551608df02378fca1793e0b3f469baf322d
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080547"
---
# <a name="case-resource-type"></a>тип ресурса case

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В контексте eDiscovery содержатся хранители, хранитель, коллекции, наборы обзоров и экспорт. Подробные сведения [см. в Advanced eDiscovery](/microsoft-365/compliance/overview-ediscovery-20).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Случай списка](../api/ediscovery-case-list.md) | [коллекция microsoft.graph.ediscovery.case](ediscovery-case.md) | Извлечение списка [объектов-кейсов.](../resources/ediscovery-case.md)|
| [Создание дела](../api/ediscovery-case-post.md) | [microsoft.graph.ediscovery.case](ediscovery-case.md) | Создайте новый **объект case.** |
| [Get case](../api/ediscovery-case-get.md) | [microsoft.graph.ediscovery.case](ediscovery-case.md) | Извлечение свойств и связей объекта **case.** |
| [Дело об обновлении](../api/ediscovery-case-update.md) | [microsoft.graph.ediscovery.case](ediscovery-case.md) | Обновим свойства **объекта-кейса.** |
| [Удаление случая](../api/ediscovery-case-delete.md) | Нет | Удаление **объекта дела.** |
| [Закрыть дело](../api/ediscovery-case-close.md)        | Нет                                              | Закрой дело об обнаружении электронной почты. Подробные сведения [см. в материале Close a case](/microsoft-365/compliance/close-or-delete-case#close-a-case). |
| [Повторное открытие дела](../api/ediscovery-case-reopen.md)      | Нет                                              | Повторное открытие закрытого дела об обнаружении электронной почты. Подробные сведения см. [в материале Reopen a closed case](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case).|
| Хранители |
| [Хранители списка](../api/ediscovery-case-list-custodians.md)   | [коллекция microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) |Получите список объектов [хранителя](../resources/ediscovery-custodian.md) и их свойств.|
| [Создание хранителя](../api/ediscovery-case-post-custodians.md)  | [microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md)           |Создайте новый [объект хранителя.](../resources/ediscovery-custodian.md) После создания объекта-хранителя необходимо создать пользовательский [список](../resources/ediscovery-usersource.md) хранителя, чтобы ссылаться на его почтовый ящик и OneDrive для бизнеса сайт.|
| Юридические точки |
| [Список legalHolds](../api/ediscovery-case-list-legalholds.md)   | [коллекция microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) | Получите [legalHolds,](../resources/ediscovery-legalhold.md) которые применяются к делу.|
| [Создание legalHold](../api/ediscovery-case-post-legalholds.md)  | [microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md)           | Создание нового [объекта legalHold.](../resources/ediscovery-legalhold.md)|
| Наборы обзоров |
| [List reviewSets](../api/ediscovery-case-list-reviewsets.md)   | [коллекция microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) | Получите список [reviewSets из](../resources/ediscovery-reviewset.md) объекта **case.**|
| [Создание reviewSet](../api/ediscovery-case-post-reviewsets.md)  | [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md)           | Создайте новый [объект reviewSet.](../resources/ediscovery-reviewset.md) В теле запроса содержится отображаемое имя набора отзывов, которое является единственным рукописным свойством.|
| Параметры кейса |
| [Получение параметров](../api/ediscovery-settings-get.md)|[microsoft.graph.ediscovery.settings](../resources/ediscovery-settings.md)|Ознакомьтесь с свойствами и отношениями объекта [microsoft.graph.ediscovery.settings.](../resources/ediscovery-settings.md) |
| [Обновление параметров](../api/ediscovery-settings-update.md)|[microsoft.graph.ediscovery.settings](../resources/ediscovery-settings.md)|Обновление свойств объекта [microsoft.graph.ediscovery.settings.](../resources/ediscovery-settings.md) |
| [resetToDefault](../api/ediscovery-settings-resettodefault.md)|Нет|Сброс всех параметров в значения по умолчанию. |
| Исходные коллекции |
| [Список sourceCollections](../api/ediscovery-case-list-sourcecollections.md)|[коллекция microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Получите [sourceCollection из](../resources/ediscovery-sourcecollection.md) **объекта-кейса.**|
| [Создание sourceCollection](../api/ediscovery-case-post-sourcecollections.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Создайте новый **объект sourceCollection.**|
| Теги |
| [Теги списка](../api/ediscovery-case-list-tags.md)|[коллекция microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Извлечение списка [объектов тегов](../resources/ediscovery-tag.md) из дела об обнаружении электронных данных.|
| [Создание тега](../api/ediscovery-case-post-tags.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Создайте новый тег для указанного случая. Теги используются в наборах обзоров при просмотре контента.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|closedBy|[identitySet](/graph/api/resources/identityset)|Пользователь, закрывавший дело.|
|closedDateTime|DateTimeOffset|Дата и время закрытия дела. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|createdBy|[identitySet](/graph/api/resources/identityset)|Пользователь, создавший дело.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|description|String|Описание случая.|
|displayName|String|Имя случая.|
|externalId|String|Внешний номер случая для клиентской ссылки.|
|id|String| ID для дела об обнаружении электронной почты. Только для чтения. |
|lastModifiedBy|[identitySet](/graph/api/resources/identityset)|Последний пользователь, который изменил сущность.|
|lastModifiedDateTime|DateTimeOffset| Последняя дата и время изменения дела. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|status|microsoft.graph.ediscovery.caseStatus| Состояние дела. Возможные значения `unknown` : , , , , , и `active` `pendingDelete` `closing` `closed` `closedWithError` . Подробные сведения см. в следующей таблице.|

### <a name="casestatus-values"></a>значения caseStatus

|Member|Описание|
|:----|-----------|
| unknown | Состояние дела неизвестно. |
| active | Случай активен. |
| pendingDelete | Дело было удалено, но удаление не было полностью реализовано. |
| закрытие | Дело было закрыто, но операция не была полностью завершена. |
| закрыто | Дело закрыто. |
| closedWithError | Дело закрыто, но в деле были ошибки, высвободающие четы. |

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|хранители|[коллекция microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md)| Возвращает список объектов **хранителя для** этого **дела.**  Допускается значение null.|
|legalHolds|[коллекция microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md)| Возвращает список объектов **legalHold для** этого **дела.**  Допускается значение null. |
|noncustodialDataSources|[коллекция microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md)| Возвращает список объектов **noncustodialDataSource** для этого **случая.**  Допускается значение null. |
|operations|[коллекция microsoft.graph.ediscovery.caseOperation](../resources/ediscovery-caseoperation.md)| Возвращает список объектов операции **в** этом **случае.** Допускается значение null. |
|reviewSets|[коллекция microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md)| Возвращает список объектов **reviewSet** в этом случае. Только для чтения. Допускается значение null. |
|Settings|[коллекция microsoft.graph.ediscovery.settings](../resources/ediscovery-settings.md)| Возвращает список объектов **параметров** в этом случае. Только для чтения. Допускается значение null. |
|sourceCollections|[коллекция microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Возвращает список объектов **sourceCollection,** связанных с этим случаем.|
|tags|[коллекция microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Возвращает список объектов **тегов,** связанных с этим случаем.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
 
  ],
  "@odata.type": "microsoft.graph.ediscovery.case"
}-->

```json
{
  "@odata.type": "#microsoft.graph.ediscovery.case",
  "description": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "closedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "closedDateTime": "String (timestamp)",
  "externalId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "case resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
