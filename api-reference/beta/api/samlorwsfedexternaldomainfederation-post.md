---
title: Создание samlOrWsFedExternalDomainFederation
description: Создание нового объекта samlOrWsFedExternalDomainFederation.
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 53d95a9f40ba3253c3c6cc7fbc8133a787de0e09
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099030"
---
# <a name="create-samlorwsfedexternaldomainfederation"></a>Создание samlOrWsFedExternalDomainFederation
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового [объекта samlOrWsFedExternalDomainFederation.](../resources/samlorwsfedexternaldomainfederation.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Domain.Read.All, Domain.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Приложение|Domain.Read.All, Domain.ReadWrite.All|

Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:

* Глобальный администратор
* Администратор внешнего поставщика удостоверений

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /directory/federationConfigurations
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON объекта [samlOrWsFedExternalDomainFederation.](../resources/samlorwsfedexternaldomainfederation.md)

В следующей таблице показаны свойства, необходимые при создании [samlOrWsFedExternalDomainFederation.](../resources/samlorwsfedexternaldomainfederation.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображение имени поставщика удостоверений на основе SAML/WS-Fed. Унаследовано от [identityProviderBase](../resources/identityproviderbase.md).|
|issuerUri|Строка|URI эмитента сервера федерации. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|metadataExchangeUri|Строка|URI конечной точки обмена метаданными, используемой для проверки подлинности из богатых клиентских приложений. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|passiveSignInUri|String|URI, на которые направляются веб-клиенты при входе в службы Azure AD. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|preferredAuthenticationProtocol|String|Предпочтительный протокол проверки подлинности. Поддерживаемые значения `saml` включают или `wsfed` . Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|signingCertificate|String|Текущий сертификат, используемый для подписывания маркеров, переданных платформа удостоверений Майкрософт. Сертификат форматируется как кодированная строка Base64 для публичной части сертификата подписи маркера федеративы IdP и должна быть совместима с классом X509Certificate2.  <br/><br/> Это свойство используется в следующих сценариях: <ul><li> если требуется опрокидывка за пределами обновления автороллевера <li>в настоящее время устанавливается новая служба федерации <li> если новый сертификат подписи маркера не присутствует в свойствах федерации после обновления сертификата службы федерации. </ul> <br/><br/> Azure AD обновляет сертификаты с помощью процесса автопроверки, в котором он пытается получить новый сертификат из метаданных службы федерации за 30 дней до истечения текущего сертификата. Если новый сертификат не доступен, Azure AD ежедневно отслеживает метаданные и обновляет параметры федерации для домена при наличии нового сертификата.|

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код ответа и `201 Created` [объект samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_samlorwsfedexternaldomainfederation_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/directory/federationConfigurations
Content-Type: application/json

{
    "@odata.type": "microsoft.graph.samlOrWsFedExternalDomainFederation",
    "issuerUri": "https://contoso.com/issuerUri",
    "displayName": "contoso display name",
    "metadataExchangeUri": "https://contoso.com/metadataExchangeUri",
    "passiveSignInUri": "https://contoso.com/signin",
    "preferredAuthenticationProtocol": "wsFed",
    "domains": [
        {
            "@odata.type": "microsoft.graph.externalDomainName",
            "id": "contoso.com"
        }
    ],
    "signingCertificate": "MIIDADCCAeigAwIBAgIQEX41y8r6"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-samlorwsfedexternaldomainfederation-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-samlorwsfedexternaldomainfederation-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-samlorwsfedexternaldomainfederation-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-samlorwsfedexternaldomainfederation-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-samlorwsfedexternaldomainfederation-from--powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProviderBase"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "id": "3c41f317-9af3-4266-8ccf-26283ceec888",
    "displayName": "contoso display name"
}
```
