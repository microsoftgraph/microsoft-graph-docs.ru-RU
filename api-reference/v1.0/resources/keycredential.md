---
title: Тип ресурса Кэйкредентиал
description: Содержит ключевые учетные данные, связанные с приложением или субъектом службы. Свойство **keyCredentials** сущностей Application и servicePrincipal является коллекцией **кэйкредентиал**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 97aab57c1ed0aa9f43536b89b49ca93a422962da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072937"
---
# <a name="keycredential-resource-type"></a>Тип ресурса Кэйкредентиал

Пространство имен: microsoft.graph

Содержит ключевые учетные данные, связанные с приложением <!--or a service principal-->. Свойство **keyCredentials** [приложения](application.md) <!--and [servicePrincipal](serviceprincipal.md)--> сущность представляет собой коллекцию **кэйкредентиал**.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|кустомкэйидентифиер|Binary| Настраиваемый идентификатор ключа |
| displayName | Строка | Понятное имя для ключа. Необязательное. |
|endDateTime|DateTimeOffset|Дата и время истечения срока действия учетных данных. Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Него значение KeyID|Guid|Уникальный идентификатор (GUID) для ключа.|
|startDateTime|DateTimeOffset|Дата и время, когда учетные данные становятся действительными. Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|type|Строка|Тип учетных данных ключа; Например, "симметричный".|
|сведений|Строка|Строка, описывающая цель, для которой можно использовать ключ; Пример: "Verify".|
|key|Двоичный| Значение для учетных данных ключа. Должно быть значением в кодировке Base 64. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

