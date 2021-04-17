---
title: тип ресурса clientCertificateAuthentication
description: Представляет конфигурацию для ирисовки клиентаCertificateAuthentication.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 69870b1160078495d3b9440260aab1f231041eef
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882485"
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
