---
title: Тип ресурса appleManagedIdentityProvider
description: Представляет поставщика удостоверений Apple в клиенте Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: ee02900b6d41695d49d7c5ee38d834c676f69603
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491194"
---
# <a name="applemanagedidentityprovider-resource-type"></a>Тип ресурса appleManagedIdentityProvider
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете настроить Apple в качестве поставщика удостоверений социальных сетей для клиента Azure AD B2C. На основе информации, которую предоставляет Apple, API создает секрет клиента. Apple нужно, чтобы секрет обновлялся каждые шесть месяцев. Потребуется изменять секрет вручную.

Этот тип наследуется от [identityProviderBase](../resources/identityproviderbase.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список](../api/identityproviderbase-list.md)|Коллекция identityProviderBase|Получение всех поставщиков удостоверений, настроенных в клиенте, включая поставщиков удостоверений Apple.|
|[Создание](../api/identityproviderbase-post-identityproviders.md)|appleManagedIdentityProvider |Создание конфигурации поставщика удостоверений Apple.|
|[Получение](../api/identityproviderbase-get.md) |appleManagedIdentityProvider |Получение свойств конфигурации поставщика удостоверений Apple.|
|[Обновление](../api/identityproviderbase-update.md)|Нет|Обновление конфигурации поставщика удостоверений Apple.|
|[удаление](../api/identityproviderbase-delete.md);|Нет|Удаление конфигурации поставщика удостоверений Apple.|
|[Перечисление доступных типов поставщиков](../api/identityproviderbase-list-availableprovidertypes.md)|Коллекция String|Получение всех типов поставщиков удостоверений, доступных в клиенте.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|developerId|Строка|Идентификатор разработчика Apple. Обязательно.|
|serviceId|Строка|Идентификатор службы Apple. Обязательно.|
|keyId|Строка|Идентификатор ключа Apple. Обязательно.|
|certificateData|Строка|Данные сертификата, являющиеся длинной строкой текста из сертификата. Могут иметь значение NULL.|
|id|String|Идентификатор поставщика удостоверений. Унаследовано от [identityProviderBase](../resources/identityproviderbase.md). Только для чтения.|
|displayName|String|Отображаемое имя поставщика удостоверений. Унаследовано от [identityProviderBase](../resources/identityproviderbase.md).|

Вы можете найти developerId, serviceId, keyId и certificateData на портале разработчика Apple. Дополнительные сведения см. в руководстве по [созданию приложения Apple ID](/azure/active-directory-b2c/identity-provider-apple-id?pivots=b2c-user-flow#create-an-apple-id-application)

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider"
} -->

```json
{
    "id": "String",
    "displayName": "String",
    "developerId": "String",
    "serviceId": "String",
    "keyId": "String",
    "certificateData": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-03-30 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "appleIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
