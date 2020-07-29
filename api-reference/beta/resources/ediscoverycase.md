---
title: Тип ресурса Едисковерикасе
description: случаи обнаружения электронных данных — это контейнеры, содержащие custodians, удержания, коллекции, обзоры и экспорты.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 930d04449f24d05d8c9225869506bfc1ed2720aa
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510324"
---
# <a name="ediscoverycase-resource-type"></a>Тип ресурса Едисковерикасе

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

случаи обнаружения электронных данных — это контейнеры, содержащие custodians, удержания, коллекции, обзоры и экспорты.  Узнайте больше о обращениях и [Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/overview-ediscovery-20).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/ediscoverycase-list.md) | Коллекция [едисковерикасе](ediscoverycase.md) | Получение списка дел eDiscovery.|
| [получение](../api/ediscoverycase-get.md); | [едисковерикасе](ediscoverycase.md) | Считывание свойств дел eDiscovery. |
| [создание](../api/ediscoverycase-post.md); | [едисковерикасе](ediscoverycase.md) | Создание нового **едисковерикасе** путем публикации в коллекции вариантов. |
| [обновление](../api/ediscoverycase-update.md). | [едисковерикасе](ediscoverycase.md) | Обновление случая обнаружения электронных данных. |
| [удаление](../api/ediscoverycase-delete.md); | Нет | Удаление случая обнаружения электронных данных. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|клоседби|[identitySet](https://docs.microsoft.com/graph/api/resources/identityset)|Пользователь, который закрыл обращение.|
|closedDateTime|DateTimeOffset|Дата и время закрытия обращения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|createdBy|[identitySet](https://docs.microsoft.com/graph/api/resources/identityset)|Пользователь, создавший обращение.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|description|Строка|Описание варианта.|
|displayName|Строка|Имя дела.|
|externalId|String|Номер внешнего обращения для ссылки на клиента.|
|id|Строка| Идентификатор для случая обнаружения электронных данных. Только для чтения. |
|lastModifiedBy|[identitySet](https://docs.microsoft.com/graph/api/resources/identityset)|Последний пользователь, изменившего объект.|
|lastModifiedDateTime|DateTimeOffset| Дата и время последнего изменения обращения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|status|String| Состояние обращения. Возможные значения: `unknown` , `active` , `pendingDelete` , `closing` , `closed` и `closedWithError` . Дополнительные сведения см. в приведенной ниже таблице.|

### <a name="casestatus-values"></a>значения Касестатус

|Member|Описание|
|:----|-----------|
| unknown | Состояние обращения неизвестно. |
| ASP | Регистр активен. |
| пендингделете | Обращение было удалено, но удаление не было полностью транзакционным. |
| крываем | Обращение было закрыто, но операция не была полностью транзакционной. |
| замкнут | Обращение закрывается. |
| клоседвисеррор | Обращение закрыто, но в этом случае возникли ошибки. |

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|Обзор наборов|Коллекция [reviewing](reviewset.md)| Коллекция наборов проверки в случае. Только для чтения. Допускается значение null. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
 
  ],
  "@odata.type": "microsoft.graph.ediscoveryCase"
}-->

```json
{
  "closedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "closedDateTime": "String (timestamp)",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "id": "String (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "status": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ediscoveryCase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
