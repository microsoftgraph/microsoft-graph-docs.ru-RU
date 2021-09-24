---
title: Обновление samlOrWsFedExternalDomainFederation
description: Обновление свойств объекта samlOrWsFedExternalDomainFederation.
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b5997fc1a2f3d4f47d03b2c37df8c87a09419477
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508654"
---
# <a name="update-samlorwsfedexternaldomainfederation"></a>Обновление samlOrWsFedExternalDomainFederation
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [samlOrWsFedExternalDomainFederation.](../resources/samlorwsfedexternaldomainfederation.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Domain.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Приложение|Domain.ReadWrite.All|

Учетная запись для работы или школы должна принадлежать одной из следующих ролей Azure Active Directory [(Azure AD):](/azure/active-directory/roles/permissions-reference)

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
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса предопределять объект JSON одним или более свойствами, которые необходимо обновить для [объекта samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) в клиенте Azure AD.

В следующей таблице показаны свойства, которые можно обновить для [объекта samlOrWsFedExternalDomainFederation.](../resources/samlorwsfedexternaldomainfederation.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображение имени поставщика удостоверений на основе SAML/WS-Fed. Унаследовано от [identityProviderBase](../resources/identityproviderbase.md).|
|issuerUri|String|URI эмитента сервера федерации. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|metadataExchangeUri|String|URI конечной точки обмена метаданными, используемой для проверки подлинности из богатых клиентских приложений. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|passiveSignInUri|String|URI, на которые направляются веб-клиенты при входе в службы Azure AD. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|preferredAuthenticationProtocol|String|Предпочтительный протокол проверки подлинности. Поддерживаемые значения `saml` включают или `wsfed` . Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|signingCertificate|String|Текущий сертификат, используемый для подписывания маркеров, переданных платформа удостоверений Майкрософт. Сертификат форматируется как кодированная строка Base64 для публичной части сертификата подписи маркера федеративы IdP и должна быть совместима с классом X509Certificate2.  <br/><br/> Это свойство используется в следующих сценариях: <ul><li> если требуется опрокидывка за пределами обновления автороллевера <li>в настоящее время устанавливается новая служба федерации <li> если новый сертификат подписи маркера не присутствует в свойствах федерации после обновления сертификата службы федерации. </ul> <br/><br/> Azure AD обновляет сертификаты с помощью процесса автопроверки, в котором он пытается получить новый сертификат из метаданных службы федерации за 30 дней до истечения текущего сертификата. Если новый сертификат не доступен, Azure AD ежедневно отслеживает метаданные и обновляет параметры федерации для домена при наличии нового сертификата.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) в тексте ответа.

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
