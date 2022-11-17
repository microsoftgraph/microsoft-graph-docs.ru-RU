---
title: Обновление internalDomainFederation
description: Обновление свойств объекта internalDomainFederation.
author: akgoel23
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5498cc69bde517632af1bc481240f962be03b1a3
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447466"
---
# <a name="update-internaldomainfederation"></a>Обновление internalDomainFederation
Пространство имен: microsoft.graph

Обновление свойств объекта [internalDomainFederation](../resources/internaldomainfederation.md) .

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
PATCH /domains/{domainsId}/federationConfiguration/{internalDomainFederationId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Свойство|Тип|Описание|
|:---|:---|:---|
|activeSignInUri|String|URL-адрес конечной точки, используемой активными клиентами при проверке подлинности с помощью федеративных доменов, настроенного для единого входа в Azure Active Directory (Azure AD). Соответствует свойству **ActiveLogOnUri** [командлета Set-MsolDomainFederationSettings MSOnline v1 PowerShell](/powershell/module/msonline/set-msoldomainfederationsettings).|
|displayName|String|Отображаемое имя федеративного поставщика удостоверений (IdP). |
|federatedIdpMfaBehavior|federatedIdpMfaBehavior|Определяет, принимает ли Azure AD многофакторную проверку подлинности, выполняемую федеративным IdP, когда федеративный пользователь имеет доступ к приложению, которое управляется политикой условного доступа, требуемой MFA. Допустимые значения: `acceptIfMfaDoneByFederatedIdp`, `enforceMfaByFederatedIdp`, `rejectMfaByFederatedIdp`, `unknownFutureValue`. Дополнительные сведения см. в [разделе federatedIdpMfaBehavior.](#federatedidpmfabehavior-values)|
|isSignedAuthenticationRequestRequired|Логическое|Если `true`запросы на проверку подлинности SAML отправляются федеративному поставщику удостоверений SAML, Azure AD подписывать эти запросы с помощью ключа подписи OrgID. Если `false` (по умолчанию) запросы проверки подлинности SAML, отправленные федеративному поставщику удостоверений, не подписыются.|
|IssuerUri|String|URI издателя сервера федерации.|
|metadataExchangeUri|String|URI конечной точки обмена метаданными, используемой для проверки подлинности из полнофункциональных клиентских приложений.|
|nextSigningCertificate|String|Резервный сертификат подписи маркера, используемый для подписи маркеров по истечении срока действия основного сертификата подписи. Форматированные в виде строк в кодировке Base64 открытой части сертификата подписи маркера федеративного IdP. Должен быть совместим с классом X509Certificate2. Как и **в случае с signingCertificate**, свойство **nextSigningCertificate** используется, если требуется смена за пределами обновления автоматической смены, настраивается новая служба федерации или если новый сертификат подписи маркера отсутствует в свойствах федерации после обновления сертификата службы федерации.|
|passiveSignInUri|String|Универсальный код ресурса (URI), на который направляются веб-клиенты при входе Azure AD служб. |
|preferredAuthenticationProtocol|authenticationProtocol|Предпочтительный протокол проверки подлинности. Допустимые значения: `wsFed`, `saml`, `unknownFutureValue`. |
|promptLoginBehavior|promptLoginBehavior|Задает предпочтительное поведение для запроса на вход. Допустимые значения: `translateToFreshPasswordAuthentication`, `nativeSupport`, `disabled`, `unknownFutureValue`.|
|signingCertificate|String|Текущий сертификат, используемый для подписи маркеров, передаваемых платформа удостоверений Майкрософт. Сертификат форматируется как строка в кодировке Base64 общедоступной части сертификата подписи маркера федеративного IdP и должна быть совместима с классом X509Certificate2. <br>Это свойство используется в следующих сценариях: <li> Если требуется смена за пределами обновления автоматической регистрации <li> Настраивается новая служба федерации <li> Если новый сертификат подписи маркера отсутствует в свойствах федерации после обновления сертификата службы федерации.<br>Azure AD обновляет сертификаты с помощью процесса автоматической регистрации, в котором он пытается получить новый сертификат из метаданных службы федерации за 30 дней до истечения срока действия текущего сертификата. Если новый сертификат недоступен, Azure AD отслеживает метаданные ежедневно и обновляет параметры федерации для домена, когда доступен новый сертификат. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|signingCertificateUpdateStatus|[signingCertificateUpdateStatus](../resources/signingcertificateupdatestatus.md)|Предоставляет состояние и метку времени последнего обновления сертификата подписи.|
|signOutUri|String|URI, на который клиенты перенаправляются при выходе из Azure AD служб. Соответствует свойству **LogOffUri** [командлета Set-MsolDomainFederationSettings MSOnline версии 1 PowerShell](/powershell/module/msonline/set-msoldomainfederationsettings).|

### <a name="federatedidpmfabehavior-values"></a>Значения federatedIdpMfaBehavior

| Member | Описание |
| :--- | :--- |
| acceptIfMfaDoneByFederatedIdp | Azure AD принимает MFA, выполняемый федеративным поставщиком удостоверений. Если федеративный поставщик удостоверений не выполнил MFA, Azure AD выполняет MFA. |
| enforceMfaByFederatedIdp | Azure AD принимает многофакторную проверку подлинности, выполняемую федеративным поставщиком удостоверений. Если федеративный поставщик удостоверений не выполнил MFA, он перенаправляет запрос к федеративному поставщику удостоверений для выполнения MFA. |
| rejectMfaByFederatedIdp | Azure AD выполняет многофакторную проверку подлинности и отклоняет MFA, выполняемую федеративным поставщиком удостоверений. |

>[!NOTE]
>**federatedIdpMfaBehavior** — это версия свойства **SupportsMfa** командлета [Set-MsolDomainFederationSettings MSOnline версии 1 PowerShell](/powershell/module/msonline/set-msoldomainfederationsettings). 
>+ Переключение **между federatedIdpMfaBehavior** и **SupportsMfa** не поддерживается.
>+ Если **свойство federatedIdpMfaBehavior** задано, Azure AD параметр **SupportsMfa** игнорируется.
>+ Если свойство **federatedIdpMfaBehavior** никогда не задано, Azure AD будет по-прежнему учитывать параметр **SupportsMfa**.
>+ Если ни **federatedIdpMfaBehavior**, ни **SupportsMfa** не заданы, Azure AD будет по умолчанию работать`acceptIfMfaDoneByFederatedIdp`.



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и обновленный [объект internalDomainFederation](../resources/internaldomainfederation.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_internaldomainfederation"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/domains/contoso.com/federationConfiguration/6601d14b-d113-8f64-fda2-9b5ddda18ecc
Content-Type: application/json

{
  "displayName": "Contoso name change",  
  "federatedIdpMfaBehavior": "acceptIfMfaDoneByFederatedIdp"
}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.internalDomainFederation"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.internalDomainFederation",
  "id": "6601d14b-d113-8f64-fda2-9b5ddda18ecc",
   "displayName": "Contoso name change",
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
   "federatedIdpMfaBehavior": "acceptIfMfaDoneByFederatedIdp"
}
```

