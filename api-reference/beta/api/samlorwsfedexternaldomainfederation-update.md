---
title: Обновление samlOrWsFedExternalDomainFederation
description: Обновление свойств объекта samlOrWsFedExternalDomainFederation.
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4e6f568cd2be81883086ea45aa1434f2669e0f17
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768149"
---
# <a name="update-samlorwsfedexternaldomainfederation"></a>Обновление samlOrWsFedExternalDomainFederation
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|IdentityProvider.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Приложение|IdentityProvider.ReadWrite.All|

Учетная запись рабочей или учебной учетной записи должна принадлежать одной из следующих ролей [Azure Active Directory (Azure AD).](/azure/active-directory/roles/permissions-reference)

* Глобальный администратор
* Администратор внешнего поставщика удостоверений

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH directory/federationConfigurations/graph.samlOrWsFedExternalDomainFederation/{samlOrWsFedExternalDomainFederation ID}
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса укажите объект JSON с одним или несколькими свойствами, которые необходимо обновить для объекта [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) в Azure AD клиенте.

В следующей таблице показаны свойства, которые можно обновить для объекта [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) .

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя поставщика удостоверений на основе SAML/WS-Fed. Унаследовано от [identityProviderBase](../resources/identityproviderbase.md).|
|IssuerUri|String|URI издателя сервера федерации. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|metadataExchangeUri|String|URI конечной точки обмена метаданными, используемой для проверки подлинности из полнофункциональных клиентских приложений. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|passiveSignInUri|String|Универсальный код ресурса (URI), на который направляются веб-клиенты при входе в Azure AD служб. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|preferredAuthenticationProtocol|String|Предпочтительный протокол проверки подлинности. Поддерживаемые значения включают или `saml` `wsfed`. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|signingCertificate|String|Текущий сертификат, используемый для подписи маркеров, передаваемых платформа удостоверений Майкрософт. Сертификат форматируется как строка в кодировке Base64 общедоступной части сертификата подписи маркера федеративного IdP и должна быть совместима с классом X509Certificate2.  <br/><br/> Это свойство используется в следующих сценариях: <ul><li> Значение , если требуется смена за пределами обновления автоматической регистрации. <li>настраивается новая служба федерации; <li> Значение , если новый сертификат подписи маркера отсутствует в свойствах федерации после обновления сертификата службы федерации. </ul> <br/><br/> Azure AD обновляет сертификаты с помощью процесса автоматической регистрации, в котором он пытается получить новый сертификат из метаданных службы федерации за 30 дней до истечения срока действия текущего сертификата. Если новый сертификат недоступен, Azure AD отслеживает метаданные ежедневно и обновляет параметры федерации для домена, когда доступен новый сертификат.|

## <a name="response"></a>Отклик

В случае успешного `200 OK` выполнения этот метод возвращает код отклика и обновленный объект [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_samlorwsfedexternaldomainfederation"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/directory/federationConfigurations/graph.samlOrWsFedExternalDomainFederation/d5a56845-6845-d5a5-4568-a5d54568a5d5
Content-Type: application/json

{
  "displayName": "Contoso name change",
  "issuerUri": "http://contoso-test.com/adfs/services/trust",
  "metadataExchangeUri": null,
  "signingCertificate": "M66C6DCCAdCgAwIBAgIQQ6vYJIVKQ",
  "passiveSignInUri": "https://contoso-test.com/adfs/ls/",
  "preferredAuthenticationProtocol": "wsFed"
}


```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-samlorwsfedexternaldomainfederation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-samlorwsfedexternaldomainfederation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-samlorwsfedexternaldomainfederation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-samlorwsfedexternaldomainfederation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
 "id": "d5a56845-6845-d5a5-4568-a5d54568a5d5",
  "displayName": "Contoso name change",
  "issuerUri": "http://contoso-test.com/adfs/services/trust",
  "metadataExchangeUri": null,
  "signingCertificate": "M66C6DCCAdCgAwIBAgIQQ6vYJIVKQ",
  "passiveSignInUri": "https://contoso-test.com/adfs/ls/",
  "preferredAuthenticationProtocol": "wsFed",
  "domains": [
      {
          "id": "contoso.com"
      }
  ]
}
```
