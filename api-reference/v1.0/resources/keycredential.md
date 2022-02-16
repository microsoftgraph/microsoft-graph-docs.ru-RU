---
title: тип ресурса keyCredential
description: Содержит ключевые учетные данные, связанные с приложением или директором службы. Свойство **keyCredentials** сущностями приложения и servicePrincipal — это коллекция **keyCredential**.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: madansr7
ms.openlocfilehash: 18a96212ca00ad211d1e1848cbfa5e73c552501f
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/16/2022
ms.locfileid: "62853237"
---
# <a name="keycredential-resource-type"></a>тип ресурса keyCredential

Пространство имен: microsoft.graph

Содержит ключевые учетные данные, связанные с приложением или директором службы. Свойство **keyCredentials** сущностями [приложения](application.md) и [servicePrincipal](serviceprincipal.md) — это коллекция **keyCredential**.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binary| Настраиваемый идентификатор ключа |
| displayName | Строка | Удобное имя для ключа. Необязательное свойство. |
|endDateTime|DateTimeOffset|Дата и время истечения срока действия учетных данных. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|key|Двоичный| Необработанные данные сертификата в массиве byte преобразованы в строку Base64. Возвращается только для `$select` одного объекта, то есть `GET applications/{applicationId}?$select=keyCredentials` , или `GET servicePrincipals/{servicePrincipalId}?$select=keyCredentials`, в противном случае, это всегда `null`. |
|keyId|GUID|Уникальный идентификатор (GUID) для ключа.|
|startDateTime|DateTimeOffset|Дата и время, в течение которых учетные данные становятся действительными. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|type|String|Тип учетных данных ключей; например, `Symmetric`. `AsymmetricX509Cert`|
|использование|Строка|Строка, описываемая цель, для которой можно использовать ключ; например, `Verify`.|

## <a name="json-representation"></a>Представление JSON

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
  "keyId": "GUID",
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

