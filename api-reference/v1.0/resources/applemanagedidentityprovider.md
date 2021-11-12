---
title: Тип ресурса appleManagedIdentityProvider
description: Представляет поставщика удостоверений Apple в клиенте Azure AD B2C.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: ce307ea651515482c6c82baa91c8fe4dcd598219
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60891248"
---
# <a name="applemanagedidentityprovider-resource-type"></a>Тип ресурса appleManagedIdentityProvider
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет поставщика удостоверений Apple в клиенте Azure AD B2C.

Вы можете настроить Apple в качестве поставщика удостоверений социальных сетей для клиента Azure AD B2C. На основе информации, которую предоставляет Apple, API создает секрет клиента. Apple нужно, чтобы секрет обновлялся каждые шесть месяцев. Вам придется изменять секрет вручную.

Наследуется от [identityProviderBase](../resources/identityproviderbase.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список](../api/identitycontainer-list-identityproviders.md)|Коллекция [identityProviderBase](../resources/identityproviderbase.md)|Извлечение всех поставщиков удостоверений, настроенных в клиенте, включая поставщиков удостоверений Apple. Нет существует способа получить только поставщиков удостоверений Apple в клиенте.|
|[Создание](../api/identitycontainer-post-identityproviders.md)|[appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) |Создание конфигурации поставщика удостоверений Apple.|
|[Получение](../api/identityproviderbase-get.md) |[appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) |Получение свойств конфигурации поставщика удостоверений Apple.|
|[Обновление](../api/identityproviderbase-update.md)|Нет|Обновление конфигурации поставщика удостоверений Apple.|
|[удаление](../api/identityproviderbase-delete.md);|Нет|Удаление конфигурации поставщика удостоверений Apple.|
|[Перечисление доступных типов поставщиков](../api/identityproviderbase-availableprovidertypes.md)|Коллекция String|Получение всех типов поставщиков удостоверений, доступных в клиенте.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|certificateData|Строка|Данные сертификата, который является длинной строкой текста из сертификата. Может быть null.|
|developerId|Строка|Идентификатор разработчика Apple. Обязательно.|
|displayName|String|Отображаемое имя поставщика удостоверений. Наследуется от [identityProviderBase](../resources/identityproviderbase.md).|
|id|String|Идентификатор поставщика удостоверений. Наследуется от [identityProviderBase](../resources/identityproviderbase.md). Только для чтения.|
|keyId|Строка|Идентификатор ключа Apple. Обязательно.|
|serviceId|Строка|Идентификатор службы Apple. Обязательно.|

Получение **developerId,** **serviceId,** **keyId** и **certificateData** с портала разработчика Apple. Дополнительные сведения можно получить в руководстве по [созданию приложения Apple ID.](/azure/active-directory-b2c/identity-provider-apple-id?pivots=b2c-user-flow#create-an-apple-id-application)

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
