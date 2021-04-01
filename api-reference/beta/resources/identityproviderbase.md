---
title: Тип ресурса identityProviderBase
description: Представляет поставщиков удостоверений в клиенте Azure Active Directory и клиенте Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 1a3d26697c26b803bcbac9141d7ff011575f91f7
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491209"
---
# <a name="identityproviderbase-resource-type"></a>Тип ресурса identityProviderBase
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет поставщиков удостоверений с [внешними удостоверениями](/azure/active-directory/external-identities/) для клиента Azure Active Directory и клиента Azure AD B2C.

Для сценариев Azure AD B2B в каталоге Azure AD поставщиком удостоверений может быть [socialIdentityProvider](../resources/socialidentityprovider.md) или [builtinIdentityProvider](../resources/builtinidentityprovider.md), наследуемый от типа ресурса identityProviderBase.

Настройка поставщика удостоверений в каталоге Azure AD позволяет применять новые гостевые сценарии Azure AD B2B. Например, в организации есть ресурсы в Microsoft 365, которыми нужно поделиться с пользователем Gmail. Для проверки подлинности и доступа к документам пользователь Gmail использует данные учетной записи Google.

В каталоге Azure AD B2C типом поставщика удостоверений может быть [socialIdentityProviders](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) или [appleIdentityProvider](../resources/appleidentityprovider.md), наследуемый от типа ресурса identityProviderBase.

Настройка поставщика удостоверений в каталоге Azure AD B2C позволяет пользователям регистрироваться и входить в приложение с помощью учетных записей социальных сетей или настраиваемого поставщика, поддерживающего OpenID Connect. Например, приложение может использовать Azure AD B2C, чтобы разрешить пользователям регистрироваться в службе с помощью учетной записи Facebook или собственного поставщика удостоверений, соответствующего протоколу OIDC.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список](../api/identityproviderbase-list.md)|Коллекция identityProviderBase|Получение всех поставщиков удостоверений, настроенных в клиенте.|
|[Перечисление доступных типов поставщиков](../api/identityproviderbase-list-availableprovidertypes.md)|Коллекция String|Получение всех типов поставщиков удостоверений, доступных в клиенте.|

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
    "displayName": "String",
}
```
