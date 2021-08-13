---
title: тип ресурса apiAuthenticationConfigurationBase
description: Представляет базовый тип конфигурации проверки подлинности, используемой для вызова API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c897bc970fc4527a03593a72e1ea760ab78fc696a75180e0e718a81ab90455ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54150047"
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
