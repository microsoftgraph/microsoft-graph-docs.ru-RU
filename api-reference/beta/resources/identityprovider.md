---
title: Тип ресурса identityProvider
description: Представляет поставщиков удостоверений в клиенте Azure Active Directory и клиенте Azure AD B2C.
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: a04c5fcf709da10a1b7b1c37d4d81097e656bc4a
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695310"
---
# <a name="identityprovider-resource-type-deprecated"></a>Тип ресурса identityProvider (нерекомендуемый)
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

Представляет поставщиков удостоверений с [внешними удостоверениями](/azure/active-directory/external-identities/) для клиента Azure Active Directory и клиента Azure AD B2C.

Для сценариев Azure AD B2B в клиенте Azure AD типом поставщика удостоверений может быть Google или Facebook.

Настройка поставщика удостоверений в клиенте Azure AD позволяет применять новые гостевые сценарии Azure AD B2B. Например, в организации есть ресурсы в Microsoft 365, которыми нужно поделиться с пользователем Gmail. Для проверки подлинности и доступа к документам пользователь Gmail использует данные учетной записи Google.

В клиенте Azure AD B2C типом поставщика удостоверений может быть **Майкрософт**, **Google**, **Facebook**, **Amazon**, **LinkedIn**, **Twitter** или любой [openIdConnectProvider](../resources/openidconnectprovider.md). В предварительной версии доступны следующие поставщики удостоверений: **Weibo**, **QQ**, **WeChat** и **GitHub**.

Настройка поставщика удостоверений в клиенте Azure AD B2C позволяет пользователям регистрироваться и входить с помощью учетных записей социальных сетей или настраиваемого поставщика, поддерживающего OpenID Connect, в приложении. Например, приложение может использовать Azure AD B2C, чтобы разрешить пользователям регистрироваться в службе с помощью учетной записи Facebook или собственного поставщика удостоверений, соответствующего протоколу OIDC.

Если это настраиваемый поставщик удостоверений OpenID Connect с `OpenIDConnect` в качестве `type`, он представляется с помощью типа ресурса [openIdConnectProvider](../resources/openidconnectprovider.md), наследуемого от типа ресурса identityProvider.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление](../api/identityprovider-list.md)|Коллекция объектов identityProvider|Получение всех поставщиков удостоверений, настроенных в клиенте.|
|[Создание](../api/identityprovider-post-identityproviders.md)|identityProvider|Создание поставщика удостоверений.|
|[Получение](../api/identityprovider-get.md) |identityProvider|Получение свойств поставщика удостоверений.|
|[Обновление](../api/identityprovider-update.md)|Нет|Обновление поставщика удостоверений.|
|[Удаление](../api/identityprovider-delete.md)|Нет|Удаление поставщика удостоверений.|
|[Перечисление доступных типов поставщиков](../api/identityprovider-list-availableprovidertypes.md)|Коллекция String|Получение всех доступных типов поставщиков удостоверений.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|clientId|String|Идентификатор клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений. Это обязательное поле. Не допускается значение NULL.|
|clientSecret|Строка|Секрет клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений. Только для записи. Операция чтения возвращает `****`. Это поле обязательно для заполнения. Обязательно. Значение null не допускается.|
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
