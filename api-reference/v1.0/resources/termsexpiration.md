---
title: тип ресурса termsExpiration
description: Предоставляет дополнительные параметры для запланированного истечения срока действия соглашения.
localization_priority: Normal
ms.prod: governance
author: raprakasMSFT
doc_type: resourcePageType
ms.openlocfilehash: cd1e7f437e8bf942d69368bc4c78410eed95dd2e42ac0a0f0dd77319578d0991
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54174873"
---
# <a name="termsexpiration-resource-type"></a>тип ресурса termsExpiration

Пространство имен: microsoft.graph

Предоставляет дополнительные параметры для запланированного истечения срока действия соглашения.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| startDateTime|DateTimeOffset | DateTime, когда срок действия соглашения истекает для всех пользователей. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".|
| частота| Длительность | Представляет частоту, с которой срок действия терминов истекает после его первого истечения, как установлено **в startDateTime.** Значение представлено в формате ISO 8601 для длительности. Например, `PT1M` представляет период времени 1 месяц.|

## <a name="json-representation"></a>Представление JSON

Ниже приводится представление JSON этого ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.termsExpiration",
}-->

```json
{
   "startDateTime": "2018-10-01T00:00:00.0000000Z",
   "frequency": "Duration"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "termsExpiration complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


