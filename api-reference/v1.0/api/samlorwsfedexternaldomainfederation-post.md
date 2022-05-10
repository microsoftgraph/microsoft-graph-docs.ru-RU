---
title: Создание samlOrWsFedExternalDomainFederation
description: Создайте объект samlOrWsFedExternalDomainFederation.
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: efe267c3c8f5a008258939e3b586cd9e97924dc3
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296639"
---
# <a name="create-samlorwsfedexternaldomainfederation"></a>Создание samlOrWsFedExternalDomainFederation
Пространство имен: microsoft.graph

Создайте объект [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Domain.Read.All, Domain.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Приложение|Domain.Read.All, Domain.ReadWrite.All|

Учетная запись рабочей или учебной учетной записи должна принадлежать к одной из следующих ролей:

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

В тексте запроса добавьте представление объекта [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) в формате JSON.

В следующей таблице показаны свойства, необходимые при создании [объекта samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя поставщика удостоверений на основе SAML/WS-Fed. Унаследовано от [identityProviderBase](../resources/identityproviderbase.md).|
|IssuerUri|Строка|URI издателя сервера федерации. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|metadataExchangeUri|Строка|URI конечной точки обмена метаданными, используемой для проверки подлинности из полнофункциональных клиентских приложений. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|passiveSignInUri|Строка|Универсальный код ресурса (URI), на который направляются веб-клиенты при входе в Azure AD служб. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|preferredAuthenticationProtocol|authenticationProtocol|Предпочтительный протокол проверки подлинности. Возможные значения: `wsFed`, `saml`. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|signingCertificate|Строка|Текущий сертификат, используемый для подписи маркеров, передаваемых платформа удостоверений Майкрософт. Сертификат форматируется как строка в кодировке Base64 общедоступной части сертификата подписи маркера федеративного IdP и должна быть совместима с классом X509Certificate2.  <br/><br/> Это свойство используется в следующих сценариях: <ul><li> Значение , если требуется смена за пределами обновления автоматической регистрации. <li>настраивается новая служба федерации; <li> Значение , если новый сертификат подписи маркера отсутствует в свойствах федерации после обновления сертификата службы федерации. </ul> <br/><br/> Azure AD обновляет сертификаты с помощью процесса автоматической регистрации, в котором он пытается получить новый сертификат из метаданных службы федерации за 30 дней до истечения срока действия текущего сертификата. Если новый сертификат недоступен, Azure AD отслеживает метаданные ежедневно и обновляет параметры федерации для домена, когда доступен новый сертификат.|

## <a name="response"></a>Отклик

В случае успешного выполнения `201 Created` этот метод возвращает код отклика и объект [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

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
