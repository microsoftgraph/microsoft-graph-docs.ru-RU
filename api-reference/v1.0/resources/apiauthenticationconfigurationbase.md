---
title: тип ресурса apiAuthenticationConfigurationBase
description: Представляет базовый тип конфигурации проверки подлинности, используемой для вызова API.
author: nickgmicrosoft
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3e3086ac90eabc15527a84f9c215659def06b7ea
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094480"
---
# <a name="apiauthenticationconfigurationbase-resource-type"></a>тип ресурса apiAuthenticationConfigurationBase

Пространство имен: microsoft.graph

Базовый тип для удержания сведений о проверке подлинности для вызова API.

Производные типы включают в себя:
- [basicAuthentication](basicauthentication.md) для базовой проверки подлинности HTTP
- [pkcs12certificate](pkcs12certificate.md) для проверки подлинности сертификатов клиента (используется для создания или отправки соединителя API)
- [clientCertificateAuthentication](pkcs12certificate.md) для проверки подлинности сертификатов клиента (используется для получения клиентских сертификатов соединителя API)

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.apiAuthenticationConfigurationBase"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.apiAuthenticationConfigurationBase"
}
```
