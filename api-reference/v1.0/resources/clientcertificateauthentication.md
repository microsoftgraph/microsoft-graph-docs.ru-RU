---
title: тип ресурса clientCertificateAuthentication
description: Представляет конфигурацию для ирисовки клиентаCertificateAuthentication.
author: nickgmicrosoft
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 70a3885d313f368c71ab1dc2f10c158a726ffde9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109271"
---
# <a name="clientcertificateauthentication-resource-type"></a>тип ресурса clientCertificateAuthentication

Пространство имен: microsoft.graph

Тип, полученный из apiAuthenticationConfigurationBase, который используется для представления проверки подлинности клиентского сертификата на основе Pkcs12. Это используется для получения общедоступных свойств загруженных сертификатов.

Наследует [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|certificateList| [коллекция pkcs12CertificateInformation](../resources/pkcs12CertificateInformation.md)| Список сертификатов, загруженных для этого соединиттеля API.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.clientCertificateAuthentication"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.clientCertificateAuthentication",
  "certificateList": "Collection(microsoft.graph.pkcs12CertificateInformation)",
}
```
