---
title: Тип ресурса identityProvider
description: Представляет поставщика удостоверений Azure Active Directory (Azure AD).
localization_priority: Priority
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3a8cf2d9c262551beb060c8b412c77ce50ffeeda
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444401"
---
# <a name="identityprovider-resource-type"></a>Тип ресурса identityProvider

Пространство имен: microsoft.graph

Представляет поставщика удостоверений Azure Active Directory (Azure AD). Поставщиком удостоверений может быть Майкрософт, Google, Facebook, Amazon, LinkedIn или Twitter. Поставщики удостоверений в предварительной версии: Weibo, QQ, WeChat, GitHub и любой поставщик, поддерживаемый OpenID Connect. 

Возможности для пользователей в результате настройки поставщика удостоверений в клиенте Azure AD B2C:

* Регистрация и вход с помощью учетной записи социальных сетей в пользовательском приложении. Например, приложение может использовать Azure AD B2C, чтобы разрешить пользователям регистрироваться в службе с помощью учетной записи Facebook.
* Связывание существующей локальной учетной записи с учетной записью социальной сети в пользовательском приложении. Например, пользователь создал имя пользователя и пароль (локальную учетную запись) в приложении. Затем он захотел связать существующую локальную учетную запись с новой учетной записью Facebook, чтобы входить с помощью Facebook.

Настройка поставщика удостоверений в клиенте Azure AD позволяет в будущем применять гостевые сценарии B2B. Например, в организации есть ресурсы в Microsoft 365, которыми нужно поделиться с пользователем Gmail. Для проверки подлинности и доступа к документам пользователь Gmail использует данные учетной записи Google.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение identityProvider](../api/identityprovider-get.md) |identityProvider|Чтение свойств существующего объекта identityProvider.|
|[Создание identityProvider](../api/identityprovider-post-identityproviders.md)|identityProvider|Создание объекта identityProvider.|
|[Обновление identityProvider](../api/identityprovider-update.md)|Нет|Обновление существующего объекта identityProvider.|
|[Удаление identityProvider](../api/identityprovider-delete.md)|Нет|Удаление существующего объекта identityProvider.|
|[Перечисление объектов identityProvider](../api/identityprovider-list.md)|Коллекция объектов identityProvider|Получение списка всех объектов identityProvider, настроенных в клиенте.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Обязательное|Допускается значение null|Описание|
|:---------------|:--------|:--------|:--------|:----------|
|clientId|String|Да|Нет|Идентификатор клиента для приложения. Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.|
|clientSecret|String|Да|Нет|Секрет клиента для приложения. Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений. Только для записи. Операция чтения возвращает "\*\*\*\*".|
|id|String|Нет|Нет|Идентификатор поставщика удостоверений.|
|name|String|Нет|Нет|Отображаемое имя поставщика удостоверений.|
|type|String|Да|Нет|Тип поставщика удостоверений Для сценариев B2C должно быть присвоено одно из указанных ниже значений. <ul><li/>Microsoft<li/>Google<li/>Amazon<li/>LinkedIn<li/>Facebook<li/>GitHub<li/>Twitter<li/>Weibo<li/>QQ<li/>WeChat</ul>Для сценариев B2B должно быть присвоено значение Google или Facebook.|

### <a name="where-to-get-the-client-id-and-secret"></a>Где взять идентификатор и секрет клиента

Для каждого поставщика удостоверений существует процесс создания регистрации приложения. Например, пользователи создают регистрацию приложения с помощью Facebook на сайте [developers.facebook.com](https://developers.facebook.com/). Получившийся идентификатор и секрет клиента можно передать для [создания identityProvider](../api/identityprovider-post-identityproviders.md). После этого каждый объект пользователя в каталоге можно объединить с любым поставщиком удостоверений клиента для проверки подлинности. Это позволяет пользователям входить путем ввода учетных данных на странице входа поставщика удостоверений. Маркер от поставщика удостоверений проверяется с помощью Azure AD перед выпуском клиентом маркера для приложения.

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->

```json
{
    "id": "String",
    "type": "String",
    "name": "String",
    "clientId": "String",
    "clientSecret": "String"
}
```

