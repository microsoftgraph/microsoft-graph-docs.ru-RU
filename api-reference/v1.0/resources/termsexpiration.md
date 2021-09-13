---
title: тип ресурса termsExpiration
description: Предоставляет дополнительные параметры для запланированного истечения срока действия соглашения.
ms.localizationpriority: medium
ms.prod: governance
author: raprakasMSFT
doc_type: resourcePageType
ms.openlocfilehash: a3786a922bb5bbff220836b2a24abeb519bece38
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128055"
---
# <a name="termsexpiration-resource-type"></a>тип ресурса termsExpiration

Пространство имен: microsoft.graph

Предоставляет дополнительные параметры для запланированного истечения срока действия соглашения.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| startDateTime|DateTimeOffset | DateTime, когда срок действия соглашения истекает для всех пользователей. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
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


