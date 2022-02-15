---
title: тип ресурса keyCredential
description: Содержит ключевые учетные данные, связанные с приложением или директором службы. Свойство **keyCredentials** сущностями приложения и servicePrincipal — это коллекция **keyCredential**.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: madansr7
ms.openlocfilehash: f0c92a613c234fccfd757d0144eefdb51a0ec316
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804376"
---
# <a name="keycredential-resource-type"></a>тип ресурса keyCredential

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит ключевые учетные данные, связанные с приложением или директором службы. Свойство **keyCredentials** сущностями [приложения](application.md) и [servicePrincipal](serviceprincipal.md) — это коллекция **keyCredential**.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binary| Настраиваемый идентификатор ключа |
| displayName | String | Удобное имя для ключа. Необязательное свойство. |
|endDateTime|DateTimeOffset|Дата и время истечения срока действия учетных данных. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|key|Двоичный| Значение для учетных данных ключа. Должно быть закодированное значение Base64. Возвращается только для `$select` одного объекта, то есть `GET applications/{applicationId}?$select=keyCredentials` , или `GET servicePrincipals/{servicePrincipalId}?$select=keyCredentials`, в противном случае, это всегда `null`. |
|keyId|Guid|Уникальный идентификатор для ключа.|
|startDateTime|DateTimeOffset|Дата и время, в течение которых учетные данные становятся действительными. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|type|String|Тип учетных данных ключей; например, `Symmetric`. `AsymmetricX509Cert`|
|использование|String|Строка, описываемая цель, для которой можно использовать ключ; например, `Verify`.|


## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

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


