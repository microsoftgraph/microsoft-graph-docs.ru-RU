---
title: тип ресурса apiAuthenticationConfigurationBase
description: Представляет базовый тип конфигурации проверки подлинности, используемой для вызова API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a9e48d38e7ad69d6790b3b9dddb85960c964ad91
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883319"
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
