---
title: тип ресурса samlOrWsFedProvider
description: Сведения о конфигурации для настройки поставщика удостоверений на WS-Fed saml или WS-Fed.
author: namkedia
localization_priority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9dbe48d7d2c229132dfea4b84282cadcdbcc8d7c
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697108"
---
# <a name="samlorwsfedprovider-resource-type"></a>тип ресурса samlOrWsFedProvider

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный тип, который предоставляет сведения о конфигурации для настройки поставщика удостоверений на основе WS-Fed на основе внешнего домена (IdP).

Наследуется от [identityProviderBase](../resources/identityproviderbase.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображение имени поставщика удостоверений на основе SAML/WS-Fed. Унаследовано от [identityProviderBase](../resources/identityproviderbase.md).|
|id|String|Идентификатор поставщика удостоверений. Наследуется от [сущности](../resources/entity.md).|
|issuerUri|String|URI эмитента сервера федерации.|
|metadataExchangeUri|String|URI конечной точки обмена метаданными, используемой для проверки подлинности из богатых клиентских приложений.|
|passiveSignInUri|String|URI, на которые веб-клиенты направляются при входе Azure Active Directory служб Azure AD.|
|metadataExchangeUri|String|URI конечной точки обмена метаданными, используемой для проверки подлинности из богатых клиентских приложений.|
|passiveSignInUri|String|URI, на которые направляются веб-клиенты при входе в службы Azure AD.|
|preferredAuthenticationProtocol|String|Предпочтительный протокол проверки подлинности. Поддерживаемые значения `saml` включают или `wsfed` .|
|signingCertificate|String|Текущий сертификат, используемый для подписывания маркеров, переданных платформа удостоверений Майкрософт. Сертификат форматируется как кодированная строка Base64 для публичной части сертификата подписи маркера федеративы IdP и должна быть совместима с классом X509Certificate2.  <br/><br/> Это свойство используется в следующих сценариях: <ul><li> если требуется опрокидывка за пределами обновления автороллевера <li>в настоящее время устанавливается новая служба федерации <li> если новый сертификат подписи маркера не присутствует в свойствах федерации после обновления сертификата службы федерации. </ul> <br/><br/> Azure AD обновляет сертификаты с помощью процесса автопроверки, в котором он пытается получить новый сертификат из метаданных службы федерации за 30 дней до истечения текущего сертификата. Если новый сертификат не доступен, Azure AD ежедневно отслеживает метаданные и обновляет параметры федерации для домена при наличии нового сертификата.|

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
