---
title: Тип ресурса builtInIdentityProvider
description: Представляет встроенных поставщиков удостоверений в клиенте Azure Active Directory.
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 7c8b4265da70100aa869d9dc593b8c0fe2b07cb6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019379"
---
# <a name="builtinidentityprovider-resource-type"></a>Тип ресурса builtInIdentityProvider
Пространство имен: microsoft.graph

Представляет встроенных поставщиков удостоверений с [внешними удостоверениями](/azure/active-directory/external-identities/) для клиента Azure Active Directory.

Для сценариев Azure AD B2B в клиенте Azure AD встроенным типом поставщика удостоверений может быть Azure Active Directory (AAD), учетная запись Майкрософт (MSA) или одноразовый секретный код по почте (EmailOTP).

Этот тип наследуется от [identityProviderBase](../resources/identityproviderbase.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список](../api/identitycontainer-list-identityproviders.md)|Коллекция [identityProviderBase](../resources/identityproviderbase.md)|Получение всех поставщиков удостоверений, настроенных в клиенте, включая встроенных поставщиков удостоверений. Невозможно получить только встроенных поставщиков удостоверений в клиенте.|
|[Получение](../api/identityproviderbase-get.md) |builtInIdentityProvider|Получение свойств встроенного поставщика удостоверений.|
|[Перечисление доступных типов поставщиков](../api/identityproviderbase-availableprovidertypes.md)|Коллекция String|Получение всех типов поставщиков удостоверений, доступных в клиенте.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|id|String|Идентификатор поставщика удостоверений. Наследуется от [identityProviderBase](../resources/identityproviderbase.md). Только для чтения.|
|displayName|String|Отображаемое имя поставщика удостоверений. Наследуется от [identityProviderBase](../resources/identityproviderbase.md).|
|identityProviderType|String|Тип поставщика удостоверений Возможные значения для сценария B2B: `AADSignup`, `MicrosoftAccount`, `EmailOTP`. Обязательный элемент.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.builtInIdentityProvider"
} -->

```json
{
    "id": "String",
    "identityProviderType": "String",
    "displayName": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-03-30 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "builtinIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
