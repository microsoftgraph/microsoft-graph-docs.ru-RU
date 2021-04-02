---
title: тип ресурса apiAuthenticationConfigurationBase
description: Представляет базовый тип конфигурации проверки подлинности, используемой для вызова API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 915e1c0c26cee173991d75bc46a1a0230844d2ec
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507968"
---
# <a name="apiauthenticationconfigurationbase-resource-type"></a>тип ресурса apiAuthenticationConfigurationBase

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Базовый тип для удержания сведений о проверке подлинности для вызова API.

Производные типы включают в себя:
- [basicAuthentication](basicauthentication.md) для базовой проверки подлинности HTTP
- [pkcs12certificate](pkcs12certificate.md) для проверки подлинности сертификатов клиента (используется для создания или отправки соединителя API)
- [clientCertificateAuthentication](pkcs12certificate.md) для проверки подлинности сертификатов клиента (используется для получения клиентских сертификатов соединителя API)

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|

## <a name="relationships"></a>Связи

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
