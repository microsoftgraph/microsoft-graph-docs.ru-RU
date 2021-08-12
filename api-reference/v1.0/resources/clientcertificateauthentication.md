---
title: тип ресурса clientCertificateAuthentication
description: Представляет конфигурацию для ирисовки клиентаCertificateAuthentication.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 89214a0e9c6805adc7bafa59f12b0091c89c953d4380bf3ea9b95d89ade2973b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212139"
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
