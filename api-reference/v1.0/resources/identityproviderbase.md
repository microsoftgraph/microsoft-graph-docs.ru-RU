---
title: Тип ресурса identityProviderBase
description: Представляет поставщиков удостоверений в клиенте Azure Active Directory и клиенте Azure AD B2C.
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 661c9ca5f1a76af52112d22671d02bd2c801b79f
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890173"
---
# <a name="identityproviderbase-resource-type"></a>Тип ресурса identityProviderBase
Пространство имен: microsoft.graph

Представляет поставщиков удостоверений с [внешними удостоверениями](/azure/active-directory/external-identities/) как для клиентов Azure Active Directory (Azure AD), так и для клиентов Azure AD B2C.

Для сценариев Azure AD B2B в каталоге Azure AD поставщиком удостоверений может быть [socialIdentityProvider](../resources/socialidentityprovider.md) или [builtinIdentityProvider](../resources/builtinidentityprovider.md). Оба наследуются от типа ресурса identityProviderBase.

Настройка поставщика удостоверений в каталоге Azure AD позволяет применять новые гостевые сценарии Azure AD B2B. Например, в организации есть ресурсы в Microsoft 365, которыми нужно поделиться с пользователем Gmail. Для проверки подлинности и доступа к документам пользователь Gmail использует данные учетной записи Google.

В каталоге Azure AD B2C типом поставщика удостоверений может быть [socialIdentityProviders](../resources/socialidentityprovider.md) или [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md), наследуемые от типа ресурса identityProviderBase.

Настройка поставщика удостоверений в каталоге Azure AD B2C позволяет пользователям регистрироваться и входить в приложение с помощью учетных записей социальных сетей или настраиваемого поставщика, поддерживающего OpenID Connect. Например, приложение может использовать Azure AD B2C, чтобы разрешить пользователям регистрироваться в службе с помощью учетной записи Facebook или собственного поставщика удостоверений, соответствующего протоколу OIDC.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список](../api/identitycontainer-list-identityproviders.md)|Коллекция [identityProviderBase](../resources/identityproviderbase.md)|Получение всех поставщиков удостоверений, настроенных в клиенте.|
|[Создание](../api/identitycontainer-post-identityproviders.md)| [socialidentityprovider](../resources/socialidentityprovider.md) или  [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) |Создайте новый объект одного из следующих типов: <br/><ul><li> [socialidentityprovider](../resources/socialidentityprovider.md) (Azure AD или Azure AD B2C) <li> [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) (Azure AD B2C) </li></ul>|
|[Получение](../api/identityproviderbase-get.md); |[socialidentityprovider](../resources/socialidentityprovider.md), [builtInIdentityProvider](../resources/builtinidentityprovider.md) или [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md)| Извлеките свойства одного из следующих типов объектов: <br/><ul><li> [socialidentityprovider](../resources/socialidentityprovider.md) (Azure AD или Azure AD B2C) <li> [builtInIdentityProvider](../resources/builtinidentityprovider.md) (Azure AD или Azure AD B2C) <li> [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) (Azure AD B2C) </li></ul>|
|[Обновление](../api/identityproviderbase-update.md)|Нет|Обновите один из следующих типов объектов: <br/><ul><li> [socialidentityprovider](../resources/socialidentityprovider.md) (Azure AD или Azure AD B2C) <li> [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) (Azure AD B2C) </li></ul>|
|[удаление](../api/identityproviderbase-delete.md);|Нет|Удалите один из следующих типов объектов: <br/><ul><li> [socialidentityprovider](../resources/socialidentityprovider.md) (Azure AD или Azure AD B2C) <li> [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) (Azure AD B2C) (Azure AD B2C)|
|[Перечисление доступных типов поставщиков](../api/identityproviderbase-availableprovidertypes.md)|Коллекция String|Извлечение всех поддерживаемых типов поставщиков удостоверений в клиенте.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|id|String|Идентификатор поставщика удостоверений.|
|displayName|String|Отображаемое имя поставщика удостоверений.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityProviderBase"
} -->

```json
{
    "id": "String",
    "displayName": "String"
}
```
