---
title: тип ресурса objectIdentity
description: Представляет удостоверение, используемого для входов в учетную запись пользователя.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: f646c2c411934b72dfe2ab0ef41d56d363466ae3
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722148"
---
# <a name="objectidentity-resource-type"></a>тип ресурса objectIdentity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет удостоверение, используемого для входов в учетную запись пользователя. Удостоверение может быть предоставлено Корпорацией Майкрософт, организациями или поставщиками социальных удостоверений, такими как Facebook, Google или Microsoft, которые привязаны к учетной записи пользователя. Это позволяет пользователю войти в учетную запись пользователя с любым из связанных удостоверений.

Свойство **удостоверений** [пользовательского ресурса](user.md) — объект **objectIdentity.**

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|signInType|Строка| Указывает типы входных данных пользователя в каталоге, такие как `emailAddress` , `userName` или `federated` . Здесь представлен уникальный идентификатор для пользователя от эмитента, который может быть в любом формате, `federated` выбранном эмитентом. Дополнительные проверки применяются в **issuerAssignedId,** когда задан тип входного знака `emailAddress` или `userName` . Это свойство также может быть заданной для любой настраиваемой строки.|
|эмитент|Строка|Указывает эмитент удостоверения, например `facebook.com` .<br>Для локальных учетных записей (где **signInType** не является) это свойство является локальным доменным именем `federated` клиента B2C по умолчанию, например `contoso.onmicrosoft.com` .<br>Для внешних пользователей из другой организации Azure AD это будет домен федерарной организации, например `contoso.com` .<br><br>Поддерживает `$filter`. Ограничение 512 символов.|
|issuerAssignedId|Строка|Указывает уникальный идентификатор, присвоенный пользователю эмитентом. Сочетание **эмитента и** **issuerAssignedId должно** быть уникальным в организации. Представляет имя входного знака для пользователя при зачете **signInType** `emailAddress` `userName` или (также известном как локальные учетные записи).<br>При **входеInType** установлено: <ul><li>`emailAddress`( или начинается `emailAddress` с `emailAddress1` типа) **issuerAssignedId** должен быть допустимым адресом электронной почты</li><li>`userName`, **issuerAssignedId** должен быть допустимой локальной [частью адреса электронной почты](https://tools.ietf.org/html/rfc3696#section-3)</li></ul>Поддерживает `$filter`. Ограничение 512 символов.|

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


