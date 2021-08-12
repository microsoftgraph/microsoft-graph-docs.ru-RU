---
title: Тип ресурса identityProviderBase
description: Представляет поставщиков удостоверений в клиенте Azure Active Directory и клиенте Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 3bd8a31e7a48e70a0ccc0631d14a7c70f595d002039aa58f332a5b1657daf0bd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152686"
---
# <a name="identityproviderbase-resource-type"></a>Тип ресурса identityProviderBase
Пространство имен: microsoft.graph

Представляет поставщиков удостоверений с [внешними удостоверениями](/azure/active-directory/external-identities/) для клиента Azure Active Directory и клиента Azure AD B2C.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список](../api/identityproviderbase-list.md)|Коллекция identityProviderBase|Получение всех поставщиков удостоверений, настроенных в клиенте.|
|[Перечисление доступных типов поставщиков](../api/identityproviderbase-list-availableprovidertypes.md)|Коллекция String|Получение всех доступных типов поставщиков удостоверений.|

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
