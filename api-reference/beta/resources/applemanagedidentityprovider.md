---
title: Тип ресурса appleManagedIdentityProvider
description: Представляет поставщика удостоверений Apple в клиенте Azure AD B2C.
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 5526b2d7d9859b064fc14c8179a45f48f2bbb76f
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696339"
---
# <a name="applemanagedidentityprovider-resource-type"></a>Тип ресурса appleManagedIdentityProvider
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете настроить Apple в качестве поставщика удостоверений социальных сетей для клиента Azure AD B2C. На основе информации, которую предоставляет Apple, API создает секрет клиента. Apple нужно, чтобы секрет обновлялся каждые шесть месяцев. Вам придется изменять секрет вручную.

Наследуется от [identityProviderBase](../resources/identityproviderbase.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список](../api/identitycontainer-list-identityproviders.md)|Коллекция [identityProviderBase](../resources/identityproviderbase.md)|Получение всех поставщиков удостоверений, настроенных в клиенте, включая поставщиков удостоверений Apple. Нет существует способа получить только поставщиков удостоверений Apple в клиенте.|
|[Создание](../api/identitycontainer-post-identityproviders.md)|[appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) |Создание конфигурации поставщика удостоверений Apple.|
|[Получение](../api/identityproviderbase-get.md) |[appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) |Получение свойств конфигурации поставщика удостоверений Apple.|
|[Обновление](../api/identityproviderbase-update.md)|Нет|Обновление конфигурации поставщика удостоверений Apple.|
|[удаление](../api/identityproviderbase-delete.md);|Нет|Удаление конфигурации поставщика удостоверений Apple.|
|[Перечисление доступных типов поставщиков](../api/identityproviderbase-availableprovidertypes.md)|Коллекция String|Получение всех типов поставщиков удостоверений, доступных в клиенте.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|developerId|Строка|Идентификатор разработчика Apple. Обязательно.|
|serviceId|Строка|Идентификатор службы Apple. Обязательно.|
|keyId|Строка|Идентификатор ключа Apple. Обязательно.|
|certificateData|Строка|Данные сертификата, являющиеся длинной строкой текста из сертификата. Могут иметь значение NULL.|
|id|String|Идентификатор поставщика удостоверений. Наследуется от [identityProviderBase](../resources/identityproviderbase.md). Только для чтения.|
|displayName|String|Отображаемое имя поставщика удостоверений. Наследуется от [identityProviderBase](../resources/identityproviderbase.md).|

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
