---
title: Создание federationConfiguration
description: Создайте объект internalDomainFederation.
author: akgoel23
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c3ec8bebe163e289dda6ecedc85a07dd9ac82440
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202496"
---
# <a name="create-federationconfiguration"></a>Создание federationConfiguration
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте объект [internalDomainFederation](../resources/internaldomainfederation.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Domain.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|Domain.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /domains/{domainsId}/federationConfiguration
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [internalDomainFederation](../resources/internaldomainfederation.md) в формате JSON.

При создании внутреннего **объектаDomainFederation** можно указать следующие свойства.

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя федеративного поставщика удостоверений.|
|IssuerUri|Строка|URI издателя сервера федерации.|
|metadataExchangeUri|Строка|URI конечной точки обмена метаданными, используемой для проверки подлинности из полнофункциональных клиентских приложений.|
|signingCertificate|Строка|Текущий сертификат, используемый для подписи маркеров, передаваемых платформа удостоверений Майкрософт. Сертификат форматируется как строка в кодировке Base64 общедоступной части сертификата подписи маркера федеративного IdP и должна быть совместима с классом X509Certificate2. <br>Это свойство используется в следующих сценариях: <li> Если требуется смена за пределами обновления автоматической регистрации <li> Настраивается новая служба федерации <li> Если новый сертификат подписи маркера отсутствует в свойствах федерации после обновления сертификата службы федерации.<br>Azure AD обновляет сертификаты с помощью процесса автоматической регистрации, в котором он пытается получить новый сертификат из метаданных службы федерации за 30 дней до истечения срока действия текущего сертификата. Если новый сертификат недоступен, Azure AD отслеживает метаданные ежедневно и обновляет параметры федерации для домена, когда доступен новый сертификат.|
|passiveSignInUri|Строка|Универсальный код ресурса (URI), на который направляются веб-клиенты при входе в Azure AD служб.|
|preferredAuthenticationProtocol|authenticationProtocol|Предпочтительный протокол проверки подлинности. Допустимые значения: `wsFed`, `saml`, `unknownFutureValue`.|
|activeSignInUri|Строка|URL-адрес конечной точки, используемой активными клиентами при проверке подлинности в федеративных доменах, настроив единый вход в Azure Active Directory (Azure AD). Соответствует свойству **ActiveLogOnUri** [командлета Set-MsolDomainFederationSettings MSOnline v1 PowerShell](/powershell/module/msonline/set-msoldomainfederationsettings).|
|signOutUri|Строка|URI, на который клиенты перенаправляются при выходе из Azure AD служб. Соответствует свойству **LogOffUri** [командлета Set-MsolDomainFederationSettings MSOnline версии 1 PowerShell](/powershell/module/msonline/set-msoldomainfederationsettings).|
|promptLoginBehavior|promptLoginBehavior|Задает предпочтительное поведение для запроса на вход. Допустимые значения: `translateToFreshPasswordAuthentication`, `nativeSupport`, `disabled`, `unknownFutureValue`.|
|isSignedAuthenticationRequestRequired|Логическое|Если значение равно true, то при отправке запросов проверки подлинности SAML федеративному поставщику удостоверений SAML Azure AD подписывать эти запросы с помощью ключа подписи OrgID. Если значение равно false (по умолчанию), запросы проверки подлинности SAML, отправленные федеративному поставщику удостоверений, не подписыются.|
|nextSigningCertificate|String|Резервный сертификат подписи маркера, используемый для подписи маркеров по истечении срока действия основного сертификата подписи. Форматированные в виде строк в кодировке Base64 открытой части сертификата подписи маркера федеративного IdP. Должен быть совместим с классом X509Certificate2. Как и **в случае с signingCertificate**, свойство **nextSigningCertificate** используется, если требуется смена за пределами обновления автоматической смены, настраивается новая служба федерации или если новый сертификат подписи маркера отсутствует в свойствах федерации после обновления сертификата службы федерации.|
|signingCertificateUpdateStatus|[signingCertificateUpdateStatus](../resources/signingcertificateupdatestatus.md)|Предоставляет состояние и метку времени последнего обновления сертификата подписи.|
|federatedIdpMfaBehavior|federatedIdpMfaBehavior|Определяет, принимает ли Azure AD многофакторную проверку подлинности, выполняемую федеративным IdP, когда федеративный пользователь имеет доступ к приложению, которое управляется политикой условного доступа, требуемой MFA. Допустимые значения: `acceptIfMfaDoneByFederatedIdp`, `enforceMfaByFederatedIdp`, `rejectMfaByFederatedIdp`, `unknownFutureValue`. Дополнительные сведения см. в [разделе federatedIdpMfaBehavior.](#federatedidpmfabehavior-values)|

### <a name="federatedidpmfabehavior-values"></a>Значения federatedIdpMfaBehavior

| Member | Описание |
| :--- | :--- |
| acceptIfMfaDoneByFederatedIdp | Azure AD принимает MFA, выполняемый федеративным поставщиком удостоверений. Если федеративный поставщик удостоверений не выполнил MFA, Azure AD выполняет MFA. |
| enforceMfaByFederatedIdp | Azure AD принимает многофакторную проверку подлинности, выполняемую федеративным поставщиком удостоверений. Если федеративный поставщик удостоверений не выполнил MFA, он перенаправляет запрос к федеративному поставщику удостоверений для выполнения MFA. |
| rejectMfaByFederatedIdp | Azure AD выполняет многофакторную проверку подлинности и отклоняет MFA, выполняемую федеративным поставщиком удостоверений. |

**Примечание.** **FederatedIdpMfaBehavior** — это версия свойства **SupportsMfa** командлета [Set-MsolDomainFederationSettings MSOnline v1 PowerShell](/powershell/module/msonline/set-msoldomainfederationsettings). 
+ Переключение **между federatedIdpMfaBehavior** и **SupportsMfa** не поддерживается.
+ После **установки свойства federatedIdpMfaBehavior** Azure AD параметр **SupportsMfa**.
+ Если свойство **federatedIdpMfaBehavior** никогда не задано, Azure AD будет по-прежнему учитывать параметр **SupportsMfa**.
+ Если ни **federatedIdpMfaBehavior**, ни **SupportsMfa** не заданы, Azure AD будет по умолчанию работать`acceptIfMfaDoneByFederatedIdp`.


## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код `201 Created` отклика и объект [internalDomainFederation](../resources/internaldomainfederation.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_internaldomainfederation_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/domains/contoso.com/federationConfiguration
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.internalDomainFederation",
  "displayName": "Contoso",
  "issuerUri": "http://contoso.com/adfs/services/trust",
  "metadataExchangeUri": "https://sts.contoso.com/adfs/services/trust/mex",
  "signingCertificate": "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI",
  "passiveSignInUri": "https://sts.contoso.com/adfs/ls",
  "preferredAuthenticationProtocol": "wsFed",
  "activeSignInUri": "https://sts.contoso.com/adfs/services/trust/2005/usernamemixed",
  "signOutUri": "https://sts.contoso.com/adfs/ls",
  "promptLoginBehavior": "nativeSupport",
  "isSignedAuthenticationRequestRequired": true,
  "nextSigningCertificate": "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI",
  "federatedIdpMfaBehavior": "rejectMfaByFederatedIdp"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-internaldomainfederation-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-internaldomainfederation-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-internaldomainfederation-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-internaldomainfederation-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-internaldomainfederation-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-internaldomainfederation-from--powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.internalDomainFederation"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.internalDomainFederation",
  "id": "6601d14b-d113-8f64-fda2-9b5ddda18ecc",
   "displayName": "Contoso",
   "issuerUri": "http://contoso.com/adfs/services/trust",
   "metadataExchangeUri": "https://sts.contoso.com/adfs/services/trust/mex",
   "signingCertificate": "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI",
   "passiveSignInUri": "https://sts.contoso.com/adfs/ls",
   "preferredAuthenticationProtocol": "wsFed",
   "activeSignInUri": "https://sts.contoso.com/adfs/services/trust/2005/usernamemixed",
   "signOutUri": "https://sts.contoso.com/adfs/ls",
   "promptLoginBehavior": "nativeSupport",
   "isSignedAuthenticationRequestRequired": true,
   "nextSigningCertificate": "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI",
   "signingCertificateUpdateStatus": {
        "certificateUpdateResult": "Success",
        "lastRunDateTime": "2021-08-25T07:44:46.2616778Z"
    },
   "federatedIdpMfaBehavior": "rejectMfaByFederatedIdp"
}
```

