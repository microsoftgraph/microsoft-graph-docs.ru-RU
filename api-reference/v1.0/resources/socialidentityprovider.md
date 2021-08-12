---
title: Тип ресурса socialIdentityProvider
description: Представляет поставщиков удостоверений социальных сетей в клиенте Azure Active Directory и клиенте Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: c5b45b142cb90eb1b7f2e43f719a2e9e9650d6b2a9917ca79c514e60a8f6fb1d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54134926"
---
# <a name="socialidentityprovider-resource-type"></a>Тип ресурса socialIdentityProvider
Пространство имен: microsoft.graph

Представляет поставщиков удостоверений социальных сетей с [внешними удостоверениями](/azure/active-directory/external-identities/) для клиента Azure Active Directory (Azure AD) и клиента Azure AD B2C.

Наследуется от [identityProviderBase](../resources/identityproviderbase.md).

Для сценариев Azure AD B2B в клиенте Azure AD типом поставщика удостоверений может быть `Google` или `Facebook`.

Настройка поставщика удостоверений в клиенте Azure AD позволяет применять новые гостевые сценарии Azure AD B2B. Например, в организации есть ресурсы в Microsoft 365, которыми нужно поделиться с пользователем Gmail. Для проверки подлинности и доступа к документам пользователь Gmail использует данные учетной записи Google.

В клиенте Azure AD B2C типом поставщика удостоверений может быть `Microsoft`, `Google`, `Facebook`, `Amazon`, `LinkedIn ` или `Twitter`. В предварительной версии доступны следующие поставщики удостоверений: `Weibo`, `QQ`, `WeChat` и `GitHub`.

Настройка поставщика удостоверений в клиенте Azure AD B2C позволяет пользователям регистрироваться и входить в приложение с помощью поставщика, поддерживающего учетные записи социальных сетей. Например, приложение может использовать Azure AD B2C, чтобы разрешить пользователям регистрироваться в службе с помощью учетной записи Facebook.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список](../api/identityproviderbase-list.md)|Коллекция [identityProviderBase](../resources/identityproviderbase.md)|Получение всех поставщиков удостоверений, настроенных в клиенте, включая поставщиков удостоверений социальных сетей.|
|[Создание](../api/identityproviderbase-post-identityproviders.md)|socialidentityprovider |Создание поставщика удостоверений.|
|[Получение](../api/identityproviderbase-get.md) |socialidentityprovider |Получение свойств поставщика удостоверений социальных сетей.|
|[Обновление](../api/identityproviderbase-update.md)|Нет|Обновление поставщика удостоверений социальных сетей.|
|[Удаление](../api/identityproviderbase-delete.md)|Нет|Удаление поставщика удостоверений социальных сетей.|
|[Перечисление доступных типов поставщиков](../api/identityproviderbase-list-availableprovidertypes.md)|Коллекция String|Получение всех типов поставщиков удостоверений, доступных в клиенте.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|clientId|String|Идентификатор для клиента приложения, полученный при регистрации приложения с помощью поставщика удостоверений. Обязательно.|
|clientSecret|String|Секрет клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений. Только для записи. Операция чтения возвращает `****`. Обязательный.|
|id|String|Идентификатор поставщика удостоверений. Унаследовано от [identityProviderBase](../resources/identityproviderbase.md). Только для чтения.|
|displayName|String|Отображаемое имя поставщика удостоверений. Наследуется от [identityProviderBase](../resources/identityproviderbase.md).|
|identityProviderType|Строка|Возможные значения для сценария B2B: `Google`, `Facebook`. Возможные значения для сценария B2C: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`, `QQ`, `WeChat`. Обязательно.|

### <a name="where-to-get-the-client-identifier-and-secret"></a>Где взять идентификатор и секрет клиента

Для каждого поставщика удостоверений существует процесс создания регистрации приложения. Например, пользователи создают регистрацию приложения с помощью Facebook на сайте [developers.facebook.com](https://developers.facebook.com/). Итоговый идентификатор и секрет клиента можно передать для [создания identityProvider](../api/identityproviderbase-post-identityproviders.md). После этого каждый объект пользователя в каталоге можно объединить с любым поставщиком удостоверений клиента для проверки подлинности. Это позволяет пользователям входить путем ввода учетных данных на странице входа поставщика удостоверений. Маркер от поставщика удостоверений проверяется с помощью Azure AD перед выпуском клиентом маркера для приложения.

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.socialIdentityProvider"
} -->

```json
{
    "id": "String",
    "identityProviderType": "String",
    "displayName": "String",
    "clientId": "String",
    "clientSecret": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "socialIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
