---
title: Тип ресурса keyCredential
description: Содержит основные учетных данных, связанных с приложением или участников-служб. Свойство **keyCredentials** сущности, приложения и servicePrincipal — это коллекция **keyCredential**.
localization_priority: Normal
ms.openlocfilehash: 0319568dad271f13b396d2f75a71839e85c96c40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851564"
---
# <a name="keycredential-resource-type"></a>Тип ресурса keyCredential

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Содержит основные учетных данных, связанных с приложением или участников-служб. Свойство **keyCredentials** сущности, [приложения](application.md) и [servicePrincipal](serviceprincipal.md) — это коллекция **keyCredential**.


## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binary| Настраиваемые идентификатор ключа |
|endDateTime|DateTimeOffset|Дата и время истечения срока действия учетных данных. Тип метки времени представляет сведения даты и времени с использованием формата ISO 8601 и — это всегда в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Идентификатор ключа|Guid|Уникальный идентификатор (GUID) для ключа.|
|startDateTime|DateTimeOffset|Дата и время, в которой действителен учетных данных. Тип метки времени представляет сведения даты и времени с использованием формата ISO 8601 и — это всегда в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|type|Строка|Тип ключа учетных данных; Например, «Симметричные».|
|об использовании|Строка|Строка, описывающая назначение, для которого можно использовать ключ; например «проверка».|
|key|Двоичный|            |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
