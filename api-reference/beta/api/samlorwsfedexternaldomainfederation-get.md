---
title: Get samlOrWsFedExternalDomainFederation
description: Ознакомьтесь с свойствами и отношениями объекта samlOrWsFedExternalDomainFederation.
author: namkedia
localization_priority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2622ab603d45fe85f2101441ea22380a80f41cc8
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697109"
---
# <a name="get-samlorwsfedexternaldomainfederation"></a>Get samlOrWsFedExternalDomainFederation
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ознакомьтесь с свойствами и отношениями [объекта samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) для определенного [внешнегоdomainName](../resources/externaldomainname.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Domain.Read.All, Domain.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Приложение|Domain.Read.All, Domain.ReadWrite.All|

Учетная запись для работы или школы должна принадлежать одной из следующих ролей Azure Active Directory [(Azure AD):](/azure/active-directory/roles/permissions-reference)

* Глобальный администратор
* Администратор внешнего поставщика удостоверений

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /directory/federationConfigurations/graph.samlOrWsFedExternalDomainFederation?$filter=domains/any(x: x/id eq 'domainName-value')
```

## <a name="query-parameters"></a>Параметры запроса

Этот метод требует `$filter` параметра запроса OData. Чтобы получить определенный [фильтр samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) на основе [externalDomainName,](../resources/externaldomainname.md)добавьте `?$filter=domains/any(x: x/id eq 'domainName-value')` . 

Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код ответа и `200 OK` [объект samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_samlorwsfedexternaldomainfederation"
}
-->

``` http
GET https://graph.microsoft.com/beta/directory/federationConfigurations/graph.samlOrWsFedExternalDomainFederation?$filter=domains/any(x: x/id eq 'contoso.com')
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.samlOrWsFedExternalDomainFederation"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
        "id": "96db02e2-80c1-5555-bc3a-de92ffb8c5be",
        "displayName": "Contoso",
        "issuerUri": "http://contoso.com/adfs/services/trust",
        "metadataExchangeUri": null,
        "signingCertificate": "MIIC6DCCAdCgAwIBAgIQQ6vYJIVKQ",
        "passiveSignInUri": "https://contoso.com/adfs/ls/",
        "preferredAuthenticationProtocol": "saml",
        "domains": [
            {
                "id": "contoso.com"
            }
        ]
    }
  ]
}

```
