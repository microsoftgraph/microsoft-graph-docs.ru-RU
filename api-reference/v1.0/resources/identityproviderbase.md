---
title: Тип ресурса identityProviderBase
description: Представляет поставщиков удостоверений в клиенте Azure Active Directory и клиенте Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 5418d78d6c124995c3783974e80343adc6bed1ea
ms.sourcegitcommit: f99dc2b6c8b4cb6f9f74cd780dccc47a2bccfaa6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2021
ms.locfileid: "58667866"
---
# <a name="identityproviderbase-resource-type"></a>Тип ресурса identityProviderBase
Пространство имен: microsoft.graph

Представляет поставщиков удостоверений с [внешними удостоверениями](/azure/active-directory/external-identities/) как для клиентов Azure Active Directory (Azure AD), так и для клиентов Azure AD B2C. Это абстрактный тип, который наследуется [socialIdentityProvider](../resources/socialidentityprovider.md) и [builtinIdentityProvider](../resources/builtinidentityprovider.md).

Для сценариев Azure AD B2B тип поставщика удостоверений — либо [socialIdentityProvider](../resources/socialidentityprovider.md), либо [builtinIdentityProvider.](../resources/builtinidentityprovider.md) Настройка поставщика удостоверений в клиенте Azure AD позволяет применять новые гостевые сценарии Azure AD B2B. Например, организация с ресурсами в Microsoft 365 может поделиться ими с пользователем Gmail. Для проверки подлинности и доступа к документам пользователь Gmail использует данные учетной записи Google.

В каталоге Azure AD B2C тип поставщика удостоверений — [socialIdentityProvider.](../resources/socialidentityprovider.md) Настройка поставщика удостоверений в каталоге Azure AD B2C позволяет пользователям регистрироваться и входить в приложение с помощью учетной записи в социальной сети. Например, приложение может использовать Azure AD B2C, чтобы разрешить пользователям регистрироваться в службе с помощью учетной записи Facebook.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список](../api/identitycontainer-list-identityproviders.md)|Коллекция [identityProviderBase](../resources/identityproviderbase.md)|Получение всех поставщиков удостоверений, настроенных в клиенте.|
|[Создание](../api/identitycontainer-post-identityproviders.md)|[socialidentityprovider](../resources/socialidentityprovider.md)|Создание [socialIdentityProvider](../resources/socialidentityprovider.md) (Azure AD или Azure AD B2C).|
|[Получение](../api/identityproviderbase-get.md) |[socialIdentityProvider](../resources/socialidentityprovider.md) или [builtinIdentityProvider](../resources/builtinidentityprovider.md)|Получение свойств [socialIdentityProvider](../resources/socialidentityprovider.md) (Azure AD или Azure AD B2C) или [builtinIdentityProvider](../resources/builtinidentityprovider.md) (Azure AD).|
|[Обновление](../api/identityproviderbase-update.md)|Нет|Обновление [socialIdentityProvider](../resources/socialidentityprovider.md) (Azure AD или Azure AD B2C).|
|[удаление](../api/identityproviderbase-delete.md);|Нет|Удаление [socialIdentityProvider](../resources/socialidentityprovider.md) (Azure AD или Azure AD B2C).|
|[Перечисление доступных типов поставщиков](../api/identityproviderbase-availableprovidertypes.md)|Коллекция String|Получение всех поддерживаемых типов поставщиков удостоверений.|

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
