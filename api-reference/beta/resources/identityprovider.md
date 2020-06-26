---
title: Тип ресурса identityProvider
description: Представляет поставщика удостоверений Azure Active Directory (Azure AD). Поставщик удостоверений может иметь значение Microsoft, Google, Facebook, Amazon или LinkedIn.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: Nickgmicrosoft
ms.openlocfilehash: 1c71fc88b4365031a126ee5c45f59de25f5fa3d9
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897059"
---
# <a name="identityprovider-resource-type"></a>Тип ресурса identityProvider

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет поставщика удостоверений Azure Active Directory (Azure AD). Поставщик удостоверений может иметь значение Microsoft, Google, Facebook, Amazon или LinkedIn.

Настройка поставщика удостоверений в клиенте B2C Azure AD позволяет:

* Пользователям выполнять вход и вход с использованием социальных учетных записей в приложении-потребителе. Например, приложение может использовать Azure AD B2C, чтобы разрешить пользователям регистрироваться в службе с помощью учетной записи Facebook.
* Пользователи могут связать существующую локальную учетную запись с социальными учетными записями в приложении-потребителе. Например, пользователь создал имя пользователя и пароль (локальную учетную запись) в приложении. Затем он захотел связать существующую локальную учетную запись с новой учетной записью Facebook, чтобы входить с помощью Facebook.

Настройка поставщика удостоверений в клиенте Azure AD позволяет в будущем применять гостевые сценарии B2B. Например, у Организации есть ресурсы в Microsoft 365, которые должны быть предоставлены пользователю Gmail. Для проверки подлинности и доступа к документам пользователь Gmail использует данные учетной записи Google.

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
|id|Строка|Нет|Нет|Идентификатор поставщика удостоверений.|
|name|String|Нет|Нет|Отображаемое имя поставщика удостоверений.|
|type|String|Да|Нет|Тип поставщика удостоверений Он должен иметь одно из следующих значений: <ul><li/>Microsoft<li/>Google<li/>Amazon<li/>LinkedIn<li/>Facebook</ul>|

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
