---
title: Тип ресурса Итемфацет
description: Тип ресурса Итемфацет
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: efd4977872dfefc5a0e5be9b10ad1fa196fa20a4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523074"
---
# <a name="itemfacet-resource-type"></a>Тип ресурса Итемфацет

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет абстрактный базовый тип, от которого наследуются все типы ресурсов в наборе EntitySet [профиля](profile.md) .

## <a name="properties"></a>Свойства

| Свойство             | Тип                            | Описание |
|:---------------------|:--------------------------------|:------------|
|алловедаудиенцес      |строка                           | Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.  |
|createdBy             |[identitySet](identityset.md)    | При первоначальном создании объекта.   |
|createdDateTime       |DateTimeOffset                   |Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id                    |String                           | Только для чтения.|
|выводов             |[инференцедата](inferencedata.md)| Содержит сведения о выводе, если объект определен. |
|lastModifiedBy        |[identitySet](identityset.md)    | Идентификатор партнера или пользователя, который последним изменил объект. |
|lastModifiedDateTime  |DateTimeOffset                   |Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemFacet",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "allowedAudiences": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "inference": {"@odata.type": "microsoft.graph.inferenceData"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemFacet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->