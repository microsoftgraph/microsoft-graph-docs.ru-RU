---
title: Тип ресурса internalDomainFederation
description: Представляет конфигурации доменов в клиенте, которые являются федеративными с Azure AD.
author: akgoel23
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: eb5788ebd83810834d19fe9500f13f11df9f6554
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447425"
---
# <a name="internaldomainfederation-resource-type"></a>Тип ресурса internalDomainFederation

Пространство имен: microsoft.graph

Представляет конфигурации доменов клиента, которые являются федеративными с Azure AD. Используйте этот ресурс для настройки параметров федерации при настройке федерации с Azure AD. Дополнительные сведения о федерации см. в статье ["Что такое федерация с Azure AD?](/azure/active-directory/hybrid/whatis-fed)".


Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание federationConfiguration](../api/domain-post-federationconfiguration.md)|[internalDomainFederation](../resources/internaldomainfederation.md)|Создайте объект [internalDomainFederation](../resources/internaldomainfederation.md) .|
|[Получение internalDomainFederation](../api/internaldomainfederation-get.md)|[internalDomainFederation](../resources/internaldomainfederation.md)|Чтение свойств и связей объекта [internalDomainFederation](../resources/internaldomainfederation.md) .|
|[Обновление internalDomainFederation](../api/internaldomainfederation-update.md)|[internalDomainFederation](../resources/internaldomainfederation.md)|Обновление свойств объекта [internalDomainFederation](../resources/internaldomainfederation.md) .|
|[Удаление internalDomainFederation](../api/internaldomainfederation-delete.md)|Нет|Удаление объекта [internalDomainFederation](../resources/internaldomainfederation.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|activeSignInUri|String|URL-адрес конечной точки, используемой активными клиентами при проверке подлинности с помощью федеративных доменов, настроенного для единого входа в Azure Active Directory (Azure AD). Соответствует свойству **ActiveLogOnUri** [командлета Set-MsolDomainFederationSettings MSOnline v1 PowerShell](/powershell/module/msonline/set-msoldomainfederationsettings).|
|displayName|String|Отображаемое имя федеративного поставщика удостоверений (IdP). Унаследовано от [identityProviderBase](../resources/identityproviderbase.md).|
|federatedIdpMfaBehavior|federatedIdpMfaBehavior|Определяет, принимает ли Azure AD многофакторную проверку подлинности, выполняемую федеративным IdP, когда федеративный пользователь имеет доступ к приложению, которое управляется политикой условного доступа, требуемой MFA. Допустимые значения: `acceptIfMfaDoneByFederatedIdp`, `enforceMfaByFederatedIdp`, `rejectMfaByFederatedIdp`, `unknownFutureValue`. Дополнительные сведения см. в [разделе federatedIdpMfaBehavior.](#federatedidpmfabehavior-values)|
|id|String|Идентификатор федеративного поставщика удостоверений. Наследуется от [сущности](../resources/entity.md).|
|isSignedAuthenticationRequestRequired|Логическое|Если `true`запросы на проверку подлинности SAML отправляются федеративному поставщику удостоверений SAML, Azure AD подписывать эти запросы с помощью ключа подписи OrgID. Если `false` (по умолчанию) запросы проверки подлинности SAML, отправленные федеративному поставщику удостоверений, не подписыются.|
|IssuerUri|String|URI издателя сервера федерации. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|metadataExchangeUri|String|URI конечной точки обмена метаданными, используемой для проверки подлинности из полнофункциональных клиентских приложений. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|nextSigningCertificate|String|Резервный сертификат подписи маркера, используемый для подписи маркеров по истечении срока действия основного сертификата подписи. Форматированные в виде строк в кодировке Base64 открытой части сертификата подписи маркера федеративного IdP. Должен быть совместим с классом X509Certificate2. Как и в случае с signingCertificate, свойство nextSigningCertificate используется, если требуется смена за пределами обновления автоматической смены, настраивается новая служба федерации или если новый сертификат подписи маркера отсутствует в свойствах федерации после обновления сертификата службы федерации.|
|passiveSignInUri|String|Универсальный код ресурса (URI), на который направляются веб-клиенты при входе Azure AD служб. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|preferredAuthenticationProtocol|authenticationProtocol|Предпочтительный протокол проверки подлинности. Допустимые значения: `wsFed`, `saml`, `unknownFutureValue`. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
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

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.internalDomainFederation",
  "baseType": "microsoft.graph.samlOrWsFedProvider",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.internalDomainFederation",
  "id": "String (identifier)",
  "displayName": "String",
  "issuerUri": "String",
  "metadataExchangeUri": "String",
  "signingCertificate": "String",
  "passiveSignInUri": "String",
  "preferredAuthenticationProtocol": "String",
  "activeSignInUri": "String",
  "signOutUri": "String",
  "promptLoginBehavior": "String",
  "isSignedAuthenticationRequestRequired": "Boolean",
  "nextSigningCertificate": "String",
  "signingCertificateUpdateStatus": {
    "certificateUpdateResult": "String",
    "@odata.type": "microsoft.graph.signingCertificateUpdateStatus"
  },
  "federatedIdpMfaBehavior": "String"
}
```

