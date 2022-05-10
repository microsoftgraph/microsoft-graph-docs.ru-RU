---
title: Тип ресурса samlOrWsFedProvider
description: Сведения о конфигурации для настройки поставщика удостоверений на WS-Fed SAML.
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0dec6cac2cdbe1bbe7f42d0d3580e82148e99ff3
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296664"
---
# <a name="samlorwsfedprovider-resource-type"></a>Тип ресурса samlOrWsFedProvider

Пространство имен: microsoft.graph

Абстрактный тип, предоставляющий сведения о конфигурации для настройки поставщика удостоверений WS-Fed или поставщика удостоверений на основе внешнего домена.

Наследуется от [identityProviderBase](../resources/identityproviderbase.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя поставщика удостоверений на основе SAML/WS-Fed. Унаследовано от [identityProviderBase](../resources/identityproviderbase.md).|
|id|String|Идентификатор поставщика удостоверений. Наследуется от [сущности](../resources/entity.md).|
|IssuerUri|Строка|URI издателя сервера федерации.|
|metadataExchangeUri|Строка|URI конечной точки обмена метаданными, используемой для проверки подлинности из полнофункциональных клиентских приложений.|
|metadataExchangeUri|Строка|URI конечной точки обмена метаданными, используемой для проверки подлинности из полнофункциональных клиентских приложений.|
|passiveSignInUri|Строка|Универсальный код ресурса (URI), на который направляются веб-клиенты при входе в Azure Active Directory (Azure AD) служб.|
|preferredAuthenticationProtocol|authenticationProtocol|Предпочтительный протокол проверки подлинности. Допустимые значения: `wsFed`, `saml`, `unknownFutureValue`.|
|signingCertificate|Строка|Текущий сертификат, используемый для подписи маркеров, передаваемых платформа удостоверений Майкрософт. Сертификат форматируется как строка в кодировке Base64 общедоступной части сертификата подписи маркера федеративного IdP и должна быть совместима с классом X509Certificate2.  <br/><br/> Это свойство используется в следующих сценариях: <ul><li> Значение , если требуется смена за пределами обновления автоматической регистрации. <li>настраивается новая служба федерации; <li> Значение , если новый сертификат подписи маркера отсутствует в свойствах федерации после обновления сертификата службы федерации. </ul> <br/><br/> Azure AD обновляет сертификаты с помощью процесса автоматической регистрации, в котором он пытается получить новый сертификат из метаданных службы федерации за 30 дней до истечения срока действия текущего сертификата. Если новый сертификат недоступен, Azure AD отслеживает метаданные ежедневно и обновляет параметры федерации для домена, когда доступен новый сертификат.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.samlOrWsFedProvider",
  "baseType": "microsoft.graph.identityProviderBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.samlOrWsFedProvider",
  "id": "String (identifier)",
  "displayName": "String",
  "issuerUri": "String",
  "metadataExchangeUri": "String",
  "signingCertificate": "String",
  "passiveSignInUri": "String",
  "preferredAuthenticationProtocol": "String"
}
```
