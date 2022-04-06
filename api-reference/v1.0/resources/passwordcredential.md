---
title: тип ресурса passwordCredential
description: Содержит учетные данные паролей, связанные с приложением или директором службы.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 48d3990e8449b82effad01cd638a17d16c356436
ms.sourcegitcommit: 0249c86925c9b4797908394c952073b5d9137911
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2022
ms.locfileid: "64477435"
---
# <a name="passwordcredential-resource-type"></a>тип ресурса passwordCredential

Пространство имен: microsoft.graph

Представляет учетные данные паролей, связанные с приложением или директором службы. Свойство **passwordCredentials** [приложения](application.md) <!--and [servicePrincipal](serviceprincipal.md) entitites--> Объект — это коллекция **объектов passwordCredential** .

> [!IMPORTANT]
> Использование POST или PATCH для набора **свойства passwordCredential** не поддерживается. Используйте следующие методы addPassword и removePassword для обновления пароля или секрета для приложения или службыPrincipal:
>
> - [приложение: addPassword](../api/application-addpassword.md)
> - [приложение: removePassword](../api/application-removepassword.md)
> - [servicePrincipal: addPassword](../api/serviceprincipal-addpassword.md)
> - [servicePrincipal: removePassword](../api/serviceprincipal-removepassword.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| customKeyIdentifier | Binary | Не следует использовать. |
| displayName | Строка | Удобное имя пароля. Необязательный аргумент. |
| endDateTime | DateTimeOffset | Дата и время, в течение которых истекает срок действия пароля, представлены в формате ISO 8601 и всегда во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Необязательный аргумент. |
| подсказка | Строка | Содержит первые три символа пароля. Только для чтения. |
| keyId | Guid | Уникальный идентификатор пароля. |
| secretText | Строка | Только для чтения; Содержит надежные пароли, созданные Azure AD длиной 16-64 символов. Сгенерированное значение пароля возвращается только во время первоначального запроса POST для [добавленияPassword](../api/application-addpassword.md). В будущем этот пароль не будет извлечен. |
| startDateTime | DateTimeOffset | Дата и время, в течение которых пароль становится допустимым. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Необязательно. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential",
  "baseType": null
}-->

```json
{
  "customKeyIdentifier": "Binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "hint": "String",
  "keyId": "Guid",
  "secretText": "String",
  "startDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

