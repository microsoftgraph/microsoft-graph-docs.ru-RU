---
title: тип ресурса samlOrWsFedExternalDomainFederation
description: Представляет федерацию SAML/WS-Fed, созданную с клиентом Azure Active Directory Azure AD
author: namkedia
localization_priority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: aee7550d2a8a098fa841056637cfc73aed5aca03
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697102"
---
# <a name="samlorwsfedexternaldomainfederation-resource-type"></a>тип ресурса samlOrWsFedExternalDomainFederation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс, позволяющий Azure Active Directory (Azure AD) настроить федерацию с другой организацией, поставщик удостоверений которой поддерживает протокол SAML или WS-Fed. Это позволяет клиенту Azure AD разрешить гостевых пользователей получать доступ к его ресурсам. Дополнительные сведения о федерации идентификаторов SAML/WS-Fed см. в федерате [Federation with SAML/WS-Fed identity providers for guest users.](/azure/active-directory/external-identities/direct-federation)

Наследует [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список samlOrWsFedExternalDomainFederations](../api/samlorwsfedexternaldomainfederation-list.md)|[коллекция samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|Получите список объектов [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) и их свойств.|
|[Создание samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-post.md)|[samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|Создание нового [объекта samlOrWsFedExternalDomainFederation.](../resources/samlorwsfedexternaldomainfederation.md)|
|[Get samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-get.md)|[samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|Ознакомьтесь с свойствами и отношениями [объекта samlOrWsFedExternalDomainFederation.](../resources/samlorwsfedexternaldomainfederation.md)|
|[Обновление samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-update.md)|[samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|Обновление свойств объекта [samlOrWsFedExternalDomainFederation.](../resources/samlorwsfedexternaldomainfederation.md)|
|[Удаление samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-delete.md)|Нет|Удаляет [объект samlOrWsFedExternalDomainFederation.](../resources/samlorwsfedexternaldomainfederation.md)|
|[Список доменов](../api/samlorwsfedexternaldomainfederation-list-domains.md)|[коллекция externalDomainName](../resources/externaldomainname.md)|Получите ресурсы externalDomainName из свойства навигации доменов.|
|[Создание externalDomainName](../api/samlorwsfedexternaldomainfederation-post-domains.md)|[externalDomainName](../resources/externaldomainname.md)|Создание нового объекта externalDomainName.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя отображения ИДП samL или WS-Fed на основе. Унаследовано от [identityProviderBase](../resources/identityproviderbase.md).|
|id|String|Идентификатор поставщика удостоверений. Наследуется от [сущности](../resources/entity.md).|
|issuerUri|String|URI эмитента сервера федерации. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|metadataExchangeUri|String|URI конечной точки обмена метаданными, используемой для проверки подлинности из богатых клиентских приложений. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|passiveSignInUri|String|URI, на которые направляются веб-клиенты при входе в службы Azure AD. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|preferredAuthenticationProtocol|String|Предпочтительный протокол проверки подлинности. Поддерживаемые значения `saml` включают или `wsfed` . Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|signingCertificate|String|Текущий сертификат, используемый для подписывания маркеров, переданных платформа удостоверений Майкрософт. Сертификат форматируется как кодированная строка Base64 для публичной части сертификата подписи маркера федеративы IdP и должна быть совместима с классом X509Certificate2.  <br/><br/> Это свойство используется в следующих сценариях: <ul><li> если требуется опрокидывка за пределами обновления автороллевера <li>в настоящее время устанавливается новая служба федерации <li> если новый сертификат подписи маркера не присутствует в свойствах федерации после обновления сертификата службы федерации. </ul> <br/><br/> Azure AD обновляет сертификаты с помощью процесса автопроверки, в котором он пытается получить новый сертификат из метаданных службы федерации за 30 дней до истечения текущего сертификата. Если новый сертификат не доступен, Azure AD ежедневно отслеживает метаданные и обновляет параметры федерации для домена при наличии нового сертификата. <br/><br/> Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|домены|[коллекция externalDomainName](../resources/externaldomainname.md)|Коллекция доменных имен внешних организаций, с помощью которых клиент федерирует. Поддерживает `$filter` (`eq`).|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.samlOrWsFedExternalDomainFederation",
  "baseType": "microsoft.graph.samlOrWsFedProvider",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.samlOrWsFedExternalDomainFederation",
  "id": "String (identifier)",
  "displayName": "String",
  "issuerUri": "String",
  "metadataExchangeUri": "String",
  "signingCertificate": "String",
  "passiveSignInUri": "String",
  "preferredAuthenticationProtocol": "String"
}
```
