---
title: Тип ресурса passwordCredential
description: Содержит учетные данные пароль, связанный с приложением или участника службы. Свойство **passwordCredentials** servicePrincipal сущности и сущности приложения — это коллекция **passwordCredential**.
ms.openlocfilehash: 79d3f76606533cf639f52ed22cd93f353e18e977
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074895"
---
# <a name="passwordcredential-resource-type"></a>Тип ресурса passwordCredential

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Содержит учетные данные пароль, связанный с приложением или участника службы. Свойство **passwordCredentials** [servicePrincipal](serviceprincipal.md) сущности и сущности [приложения](application.md) — это коллекция **passwordCredential**.


## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "secretText": "string",
  "hint": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|customKeyIdentifier|Двоичный|            |
|endDateTime|DateTimeOffset|Дата и время истечения срока действия пароля. Тип метки времени представляет сведения даты и времени с использованием формата ISO 8601 и — это всегда в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Идентификатор ключа|Guid|            |
|startDateTime|DateTimeOffset|Дата и время, в которой становится допустимый пароль. Тип метки времени представляет сведения даты и времени с использованием формата ISO 8601 и — это всегда в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|secretText|String| Пароли должны быть 16-64 символов |
|подсказка|String|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
