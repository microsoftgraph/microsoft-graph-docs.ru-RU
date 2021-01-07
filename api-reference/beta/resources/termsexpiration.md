---
title: Тип ресурса termsExpiration
description: Предоставляет дополнительные параметры при настройке запланированного срока действия соглашения.
localization_priority: Normal
ms.prod: microsoft-identity-platform
author: raprakasMSFT
doc_type: resourcePageType
ms.openlocfilehash: 5acacae700bfddcfe68431e03b2a5b03e00fed8a
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777716"
---
# <a name="termsexpiration-resource-type"></a>Тип ресурса termsExpiration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет дополнительные параметры при настройке запланированного срока действия соглашения.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| startDateTime|DateTimeOffset | Дата и время истечения срока действия соглашения для всех пользователей. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".|
| frequency| Длительность | Представляет частоту истечения срока действия терминов по истечении первого срока действия, установленного в **startDateTime.** Значение представлено в формате ISO 8601 в течение длительности. Например, `PT1M` представляет период времени 1 месяц.|

## <a name="json-representation"></a>Представление JSON

Ниже приводится представление этого ресурса в JSON.

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


