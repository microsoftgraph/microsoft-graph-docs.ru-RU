---
title: тип ресурса objectIdentity
description: Представляет удостоверение, используемого для входов в учетную запись пользователя.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: eebd9387d45ae44543e482ce8d57da61f7dfd4a4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59108893"
---
# <a name="objectidentity-resource-type"></a>тип ресурса objectIdentity

Пространство имен: microsoft.graph

Представляет удостоверение, используемого для входов в учетную запись пользователя. Удостоверение может быть предоставлено Корпорацией Майкрософт, организациями или поставщиками социальных удостоверений, такими как Facebook, Google или Microsoft, которые привязаны к учетной записи пользователя. Это позволяет пользователю войти в учетную запись пользователя с любым из связанных удостоверений.

Свойство **удостоверений** [пользовательского ресурса](user.md) — объект **objectIdentity.**

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|signInType|string| Указывает типы входных данных пользователя в каталоге, такие как `emailAddress` , `userName` или `federated` . Здесь представлен уникальный идентификатор для пользователя от эмитента, который может быть в любом формате, `federated` выбранном эмитентом. Дополнительные проверки применяются в **issuerAssignedId,** когда задан тип входного знака `emailAddress` или `userName` . Это свойство также может быть заданной для любой настраиваемой строки.|
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

