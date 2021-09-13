---
title: Тип ресурса identityProvider
description: Представляет поставщика удостоверений Azure Active Directory (Azure AD).
ms.localizationpriority: high
author: namkedia
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e6ccc49df5a96f3a7ebf16917e8eec3f075a61b3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118654"
---
# <a name="identityprovider-resource-type-deprecated"></a>Тип ресурса identityProvider (нерекомендуемый)
Пространство имен: microsoft.graph

[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

Представляет поставщика удостоверений Azure Active Directory (Azure AD). Поставщиком удостоверений может быть корпорация **Майкрософт**, **Google**, **Facebook**, **Amazon**, **LinkedIn** или **Twitter**. Поставщики удостоверений в предварительной версии: **Weibo**, **QQ**, **WeChat**, **GitHub** и любой поставщик, поддерживаемый OpenID Connect. 

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

|Свойство|Тип|Описание|
|:---------------|:--------|:--------|
|clientId|String|Идентификатор клиента для приложения. Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений. Обязательное. Не допускается значение NULL.|
|clientSecret|String|Секрет клиента для приложения. Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений. Только для записи. Операция чтения возвращает "`****`".  Обязательно. Значение null не допускается.|
|id|String|Идентификатор поставщика удостоверений.|
|name|String|Отображаемое имя поставщика удостоверений. Значение NULL не допускается.|
|type|Строка|Тип поставщика удостоверений является обязательным полем. Для сценария B2B: `Google`, `Facebook`. Для сценария B2C: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`,`QQ`, `WeChat`, `OpenIDConnect`. Значение NULL не допускается.|

### <a name="where-to-get-the-client-id-and-secret"></a>Где взять идентификатор и секрет клиента

Для каждого поставщика удостоверений существует процесс создания регистрации приложения. Например, пользователи создают регистрацию приложения с помощью Facebook на сайте [developers.facebook.com](https://developers.facebook.com/). Получившийся идентификатор и секрет клиента можно передать для [создания identityProvider](../api/identityprovider-post-identityproviders.md). После этого каждый объект пользователя в каталоге можно объединить с любым поставщиком удостоверений клиента для проверки подлинности. Это позволяет пользователям входить путем ввода учетных данных на странице входа поставщика удостоверений. Маркер от поставщика удостоверений проверяется с помощью Azure AD перед выпуском клиентом маркера для приложения.

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityProvider"
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
