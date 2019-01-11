---
title: Тип ресурса identityProvider
description: Представляет имя поставщика удостоверений Azure Active Directory (Azure AD). Поставщик удостоверений может быть Microsoft, Google, Facebook, Amazon или LinkedIn.
localization_priority: Normal
ms.openlocfilehash: 0a465b1c7b4ad7f74e6357e77da3692d64294e7e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858543"
---
# <a name="identityprovider-resource-type"></a>Тип ресурса identityProvider

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет имя поставщика удостоверений Azure Active Directory (Azure AD). Поставщик удостоверений может быть Microsoft, Google, Facebook, Amazon или LinkedIn.

Настройка поставщика удостоверений в клиент Azure AD B2C позволяет:

* Пользователи, чтобы зарегистрироваться и выполнить вход с помощью учетной записи социальных в клиентского приложения. К примеру приложение может использовать Azure AD B2C, чтобы пользователи могли подписаться на службу, используя учетную запись Facebook (en).
* Пользователям привязывать существующего локального учетную запись на социальные в клиентского приложения. Например создан пользователь имя пользователя и пароль (локальная учетная запись) в приложении. Пользователь решает более поздней версии для связывания существующей учетной записи локального своей учетной записи Facebook (en), поэтому они могут выполнить вход с помощью Facebook (en).

Настройка поставщика удостоверений в клиент Azure AD включает в будущих B2B гостя. Например, для организации имеет ресурсов в Office 365, который требуется предоставить общий доступ с пользователем Gmail. Пользователь Gmail будут использовать свои учетные данные учетной записи Google для проверки подлинности и доступ к документам.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение identityProvider](../api/identityprovider-get.md) |identityProvider|Чтение свойств существующего identityProvider.|
|[Создание identityProvider](../api/identityprovider-post-identityproviders.md)|identityProvider|Создание нового identityProvider.|
|[Обновление identityProvider](../api/identityprovider-update.md)|Нет|Обновление существующих identityProvider.|
|[Удаление identityProvider](../api/identityprovider-delete.md)|Нет|Удаление существующих identityProvider.|
|[Список identityProviders](../api/identityprovider-list.md)|identityProvider коллекции|Список всех identityProviders, настроенных в клиент.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Обязательный|Nullable|Описание|
|:---------------|:--------|:--------|:--------|:----------|
|clientId|Строка|Да|Нет|Идентификатор клиента для приложения. Это идентификатор клиента, полученные при регистрации приложения с поставщиком удостоверений.|
|clientSecret|Строка|Да|Нет|Секрет клиента для приложения. Это секрет клиента, полученные при регистрации приложения с поставщиком удостоверений. Это только для записи. Возвращает операции чтения "\*\*\*\*«.|
|id|Строка|Нет|Нет|Идентификатор поставщика удостоверений.|
|name|Строка|Нет|Нет|Отображаемое имя поставщика удостоверений.|
|type|Строка|Да|Нет|Тип поставщика удостоверений. Оно должно быть одно из следующих значений: <ul><li/>Microsoft<li/>Google<li/>Amazon<li/>LinkedIn<li/>Facebook</ul>|

### <a name="where-to-get-the-client-id-and-secret"></a>Где можно получить клиента идентификатора и секрета

Каждый поставщик удостоверений участвует в процессе создания его регистрации. Например пользователям создавать его регистрации с Facebook [developers.facebook.com](https://developers.facebook.com/). Для [создания identityProvider](../api/identityprovider-post-identityproviders.md)могут передаваться полученный идентификатор клиента и секрет клиента. Затем каждого объекта-пользователя в каталоге можно федеративными на указанные Поставщики удостоверений клиента для проверки подлинности. Это позволяет пользователю войти, введя учетные данные на поставщика удостоверений страница входа в. Маркер от поставщика удостоверений проверена Azure AD перед клиента выдает маркер для приложения.

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
