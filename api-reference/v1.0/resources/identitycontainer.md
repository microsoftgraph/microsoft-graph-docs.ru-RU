---
title: тип ресурса identityContainer
description: Представляет точку входа для различных функций внешних удостоверений для клиентов Azure Active Directory (Azure AD) и Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 7305a65f7c5e2c7ec890ac622be9885f9bb8f872
ms.sourcegitcommit: f99dc2b6c8b4cb6f9f74cd780dccc47a2bccfaa6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2021
ms.locfileid: "58668020"
---
# <a name="identitycontainer-resource-type"></a>тип ресурса identityContainer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет точку входа для различных функций во [внешних удостоверениях](/azure/active-directory/external-identities/) для клиентов Azure Active Directory (Azure AD) и Azure AD B2C.

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|apiConnectors|коллекция [identityApiConnector](identityApiConnector.md)|Представляет точку входа для соединителей API.|
|b2xUserFlows|коллекция [b2xIdentityUserFlow](b2xIdentityUserFlow.md)| Представляет точку входа для пользовательских потоков удостоверений регистрации B2X/self-service.|
|identityProvider|коллекция [identityProviderBase](identityProviderBase.md)| Представляет точку входа для базы поставщиков удостоверений.|
|userFlowAttributes|коллекция [identityUserFlowAttribute](identityUserFlowAttribute.md)| Представляет точку входа для атрибутов пользовательского потока удостоверений.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityContainer",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.identityContainer"
}
```
