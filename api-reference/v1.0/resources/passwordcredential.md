---
title: тип ресурса passwordCredential
description: Содержит учетные данные паролей, связанные с приложением или директором службы.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: fa2e05eafee60fc43d98c089e1737b69b5008fb77d0aa031d8f2c2a3d2faf245
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130018"
---
# <a name="passwordcredential-resource-type"></a>тип ресурса passwordCredential

Пространство имен: microsoft.graph

Представляет учетные данные паролей, связанные с приложением или директором службы. Свойство **passwordCredentials** [приложения](application.md) <!--and [servicePrincipal](serviceprincipal.md) entitites--> Объект — это коллекция **объектов passwordCredential.**

> [!IMPORTANT]
> Использование POST или PATCH для **набора passwordCredential** не поддерживается. Используйте методы addPassword и removePassword, чтобы обновить пароль для приложения или службыPrincipal:
>
> - [приложение: addPassword](../api/application-addpassword.md)
> - [приложение: removePassword](../api/application-removepassword.md)
> - [servicePrincipal: addPassword](../api/serviceprincipal-addpassword.md)
> - [servicePrincipal: removePassword](../api/serviceprincipal-removepassword.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| customKeyIdentifier | В двоичном формате | Не следует использовать. |
| displayName | String | Удобное имя пароля. Необязательно. |
| endDateTime | DateTimeOffset | Дата и время, в течение которых истекает срок действия пароля, представлены в формате ISO 8601 и всегда во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Необязательно. |
| подсказка | String | Содержит первые три символа пароля. Только для чтения. |
| keyId | Guid | Уникальный идентификатор пароля. |
| secretText | String | Только для чтения; Содержит надежные пароли, созданные Azure AD длиной 16-64 символов. Сгенерированное значение пароля возвращается только во время первоначального запроса POST для [добавленияPassword.](../api/application-addpassword.md) В будущем этот пароль не будет извлечен. |
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

