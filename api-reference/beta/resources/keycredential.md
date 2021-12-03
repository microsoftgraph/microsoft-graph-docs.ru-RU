---
title: тип ресурса keyCredential
description: Содержит ключевые учетные данные, связанные с приложением или директором службы. Свойство **keyCredentials** сущностями приложения и servicePrincipal — это коллекция **keyCredential**.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: madansr7
ms.openlocfilehash: 0c4e8ff5ce5f97498043e42305b05cadb7815412
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285100"
---
# <a name="keycredential-resource-type"></a>тип ресурса keyCredential

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит ключевые учетные данные, связанные с приложением или директором службы. Свойство **keyCredentials** сущностями приложения и [servicePrincipal](serviceprincipal.md) — это коллекция **keyCredential**. [](application.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binary| Настраиваемый идентификатор ключа |
| displayName | Строка | Удобное имя для ключа. Необязательно. |
|endDateTime|DateTimeOffset|Дата и время истечения срока действия учетных данных. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|key|Двоичный| Значение для учетных данных ключа. Должно быть базовым значением 64. |
|keyId|Guid|Уникальный идентификатор для ключа.|
|startDateTime|DateTimeOffset|Дата и время, в течение которых учетные данные становятся действительными. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|type|Строка|Тип учетных данных ключей; например, `Symmetric` .|
|использование|Строка|Строка, описываемая цель, для которой можно использовать ключ; например, `Verify` .|


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
  "@odata.type": "#microsoft.graph.keyCredential",
  "customKeyIdentifier": "Binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "key": "Binary",
  "keyId": "Guid",
  "startDateTime": "String (timestamp)",
  "type": "String",
  "usage": "String"
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


