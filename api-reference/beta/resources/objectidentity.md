---
title: тип ресурса objectIdentity
description: Представляет удостоверение, используемого для входов в учетную запись пользователя.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: efe27437cd1f01776445e3989c2db0b799ca14af
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764789"
---
# <a name="objectidentity-resource-type"></a>тип ресурса objectIdentity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет удостоверение, используемого для входов в учетную запись пользователя. Удостоверение может быть предоставлено Корпорацией Майкрософт, организациями или поставщиками социальных удостоверений, такими как Facebook, Google или Microsoft, которые привязаны к учетной записи пользователя. Это позволяет пользователю войти в учетную запись пользователя с любым из связанных удостоверений.

Свойство **удостоверений** [пользовательского ресурса](user.md) — объект **objectIdentity.**

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|signInType|Строка| Указывает типы входных данных пользователя в каталоге, такие как `emailAddress` , `userName` , или `federated` `userPrincipalName` . `federated` представляет уникальный идентификатор для пользователя от эмитента, который может быть в любом формате, выбранном эмитентом. Настройка или обновление `userPrincipalName` удостоверения обновят значение **свойства userPrincipalName** на объекте пользователя. Проверки, выполняемые на свойстве объекта пользователя, например проверенные домены и допустимые символы, будут выполняться при настройке или `userPrincipalName` обновлении `userPrincipalName` удостоверения. Дополнительные проверки применяются в **issuerAssignedId,** когда задан тип входного знака `emailAddress` или `userName` . Это свойство также может быть заданной для любой настраиваемой строки.|
|эмитент|string|Указывает эмитент удостоверения, например `facebook.com` .<br>Для локальных учетных записей (где **signInType** не является) это свойство является локальным доменным именем `federated` клиента B2C по умолчанию, например `contoso.onmicrosoft.com` .<br>Для внешних пользователей из другой организации Azure AD это будет домен федерарной организации, например `contoso.com` .<br><br>Поддерживает `$filter`. Ограничение 512 символов.|
|issuerAssignedId|string|Указывает уникальный идентификатор, присвоенный пользователю эмитентом. Сочетание **эмитента и** **issuerAssignedId должно** быть уникальным в организации. Представляет имя входного знака для пользователя при зачете **signInType** `emailAddress` `userName` или (также известном как локальные учетные записи).<br>При **входеInType** установлено: <ul><li>`emailAddress`, (или настраиваемая строка, которая начинается с `emailAddress` `emailAddress1` типа) **issuerAssignedId** должен быть допустимым адресом электронной почты</li><li>`userName`, **issuerAssignedId** должен быть допустимой локальной [частью адреса электронной почты](https://tools.ietf.org/html/rfc3696#section-3)</li></ul>Поддерживает `$filter`. Ограничение 100 символов.|

>**Примечание:** При фильтрации свойств **удостоверений** необходимо предоставить  как эмитент, так **и issuerAssignedId.**

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


