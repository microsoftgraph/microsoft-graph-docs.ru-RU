---
title: Тип ресурса objectIdentity
description: Представляет удостоверение, используемого для входа в учетную запись пользователя.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: 985de0fdbfa1c6ed9306ae434d128b64a7fe2aac
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094118"
---
# <a name="objectidentity-resource-type"></a>Тип ресурса objectIdentity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет удостоверение, используемого для входа в учетную запись пользователя. Удостоверение может быть предоставлено корпорацией Майкрософт, организациями или поставщиками удостоверений социальных сетей, такими как Facebook, Google или Майкрософт, которые привязаны к учетной записи пользователя. Это позволяет пользователю войти в учетную запись пользователя с любым из связанных удостоверений.

Свойство **identities** пользовательского [ресурса](user.md) является **объектом objectIdentity** .

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|signInType|Строка| Указывает типы входа пользователя в каталоге, `emailAddress`такие как , `userName`или `federated``userPrincipalName`. `federated` представляет уникальный идентификатор пользователя от издателя, который может быть в любом формате, выбранном издателем. Установка или обновление удостоверения `userPrincipalName` приведет к обновлению значения свойства **userPrincipalName** объекта пользователя. При установке `userPrincipalName` или обновлении удостоверения будут выполняться проверки свойства в объекте пользователя, например проверенные домены и допустимые `userPrincipalName` символы. Дополнительная проверка применяется к **issuerAssignedId** , если для типа входа задано значение или `emailAddress` `userName`. Этому свойству также можно задать любую пользовательскую строку.|
|Эмитента|string|Указывает издателя удостоверения, например `facebook.com`.<br>Для локальных учетных записей (где **signInType** не является `federated`) это свойство является локальным доменным именем клиента B2C по умолчанию, например `contoso.onmicrosoft.com`.<br>Для внешних пользователей из Azure AD организации это будет домен федеративной организации, например`contoso.com`.<br><br>Поддерживает `$filter`. Ограничение в 512 символов.|
|issuerAssignedId|string|Указывает уникальный идентификатор, назначенный пользователю издателем. Сочетание **издателя и** **issuerAssignedId должно** быть уникальным в пределах организации. Представляет имя входа для пользователя, если **для signInType** `emailAddress` `userName` задано значение или (также известное как локальные учетные записи).<br>Если **для signInType** задано значение: <ul><li>`emailAddress`, (или настраиваемая строка, которая начинается с `emailAddress` like `emailAddress1`) **issuerAssignedId** должен быть допустимым адресом электронной почты.</li><li>`userName`, **issuerAssignedId** должен быть допустимой [локальной частью адреса электронной почты.](https://tools.ietf.org/html/rfc3696#section-3)</li></ul>Поддерживает `$filter`. Ограничение в 100 символов.|

### <a name="filtering"></a>Фильтрация
При фильтрации по свойству **удостоверений** для **issuerAssignedId** необходимо указать и **издателя** , и **issuerAssignedId**. Кроме того:
- Для фильтрации записей с **типом signInType** `federated` требуется допустимый **издатель** и **issuerAssignedId**.
- Фильтрация записей со **значением signInType** `userName` `emailAddress` или игнорирует значение издателя. Данное поведение является особенностью продукта. 
- Фильтрация записей с **типом signInType** `userPrincipalName` не поддерживается. Это можно сделать путем фильтрации по свойству **userPrincipalName** объекта пользователя.

Фильтрация только **по издателю** поддерживается для следующих значений: `google.com`, `facebook.com`, и `mail``phone`.

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectIdentity"
}-->

```json
{
  "signInType": "string",
  "issuer": "string",
  "issuerAssignedId": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "objectIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


