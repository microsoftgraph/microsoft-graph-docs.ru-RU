---
title: тип ресурса clientCertificateAuthentication
description: Представляет конфигурацию для получения клиентаCertificateAuthentication в вызове API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0e88a1de011fb975afae49d53b8707b95e16157c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509413"
---
# <a name="clientcertificateauthentication-resource-type"></a>тип ресурса clientCertificateAuthentication

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
