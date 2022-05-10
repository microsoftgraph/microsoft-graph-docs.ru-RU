---
title: Тип ресурса samlOrWsFedExternalDomainFederation
description: Представляет способ федерации клиента Azure AD с внешней организацией, поставщик удостоверений которой поддерживает протокол SAML или WS-Fed.
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 80e9e4234af0e8ab234092968439124ff1aa23ea
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296675"
---
# <a name="samlorwsfedexternaldomainfederation-resource-type"></a>Тип ресурса samlOrWsFedExternalDomainFederation

Пространство имен: microsoft.graph

Позволяет клиенту Azure Active Directory (Azure AD) федерации с внешней организацией, поставщик удостоверений которой поддерживает протокол SAML или WS-Fed. Это позволит клиенту Azure AD предоставить доступ к своим ресурсам гостевым пользователям. Дополнительные сведения о федерации SAML или WS-Fed IdP см. в разделе "Федерация с SAMLWS-Fed поставщиках удостоверений [для гостевых пользователей.](/azure/active-directory/external-identities/direct-federation)

Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[List samlOrWsFedExternalDomainFederations](../api/samlorwsfedexternaldomainfederation-list.md)|[Коллекция samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|Получение списка объектов [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) и их свойств.|
|[Создание samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-post.md)|[samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|Создайте объект [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) .|
|[Получение samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-get.md)|[samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|Чтение свойств и связей объекта [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) .|
|[Обновление samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-update.md)|[samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|Обновление свойств объекта [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) .|
|[Удаление samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-delete.md)|Нет|Удаляет объект [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) .|
|[Список доменов](../api/samlorwsfedexternaldomainfederation-list-domains.md)|[Коллекция externalDomainName](../resources/externaldomainname.md)|Получение ресурсов externalDomainName из свойства навигации доменов.|
|[Создание externalDomainName](../api/samlorwsfedexternaldomainfederation-post-domains.md)|[externalDomainName](../resources/externaldomainname.md)|Создайте новый объект externalDomainName.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя поставщика удостоверений на WS-Fed SAML. Унаследовано от [identityProviderBase](../resources/identityproviderbase.md).|
|id|String|Идентификатор поставщика удостоверений. Наследуется от [сущности](../resources/entity.md).|
|IssuerUri|Строка|URI издателя сервера федерации. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|metadataExchangeUri|Строка|URI конечной точки обмена метаданными, используемой для проверки подлинности из полнофункциональных клиентских приложений. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|passiveSignInUri|Строка|Универсальный код ресурса (URI), на который направляются веб-клиенты при входе в Azure AD служб. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|preferredAuthenticationProtocol|authenticationProtocol|Предпочтительный протокол проверки подлинности. Допустимые значения: `wsFed`, `saml`, `unknownFutureValue`. Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|
|signingCertificate|Строка|Текущий сертификат, используемый для подписи маркеров, передаваемых платформа удостоверений Майкрософт. Сертификат форматируется как строка в кодировке Base64 общедоступной части сертификата подписи маркера федеративного IdP и должна быть совместима с классом X509Certificate2.  <br/><br/> Это свойство используется в следующих сценариях: <ul><li> Значение , если требуется смена за пределами обновления автоматической регистрации. <li>настраивается новая служба федерации; <li> Значение , если новый сертификат подписи маркера отсутствует в свойствах федерации после обновления сертификата службы федерации. </ul> <br/><br/> Azure AD обновляет сертификаты с помощью процесса автоматической регистрации, в котором он пытается получить новый сертификат из метаданных службы федерации за 30 дней до истечения срока действия текущего сертификата. Если новый сертификат недоступен, Azure AD отслеживает метаданные ежедневно и обновляет параметры федерации для домена, когда доступен новый сертификат. <br/><br/> Наследуется [от samlOrWsFedProvider](../resources/samlorwsfedprovider.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|Доменов|[Коллекция externalDomainName](../resources/externaldomainname.md)|Коллекция доменных имен внешних организаций, с которыми выполняется федерация клиента. Поддерживает `$filter` (`eq`).|

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
