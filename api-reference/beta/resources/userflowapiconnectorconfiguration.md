---
title: Тип ресурса userFlowApiConnectorConfiguration
description: Представляет, какие соединители API включены для пользовательского потока.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9f8e9732759a609eabb6733629a97c82afaba364
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132981"
---
# <a name="userflowapiconnectorconfiguration-resource-type"></a>Тип ресурса userFlowApiConnectorConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет, какие API-интерфейсы будут вызваны в определенных точках пользовательского потока.  Каждая связь этого объекта соответствует определенному шагу в пользовательском потоке, который можно настроить для вызова соединители API.

## <a name="relationships"></a>Связи

| Связь            | Тип                                            | Описание                                                                                                                                             |
| :---------------------- | :---------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
| postFederationSignup    | [identityApiConnector](identityapiconnector.md) | Указывает API, который будет вызываться после федерации с внешним поставщиком удостоверений (например, Google, Facebook или Azure AD), после регистрации пользователя (не применяется для регистрации). |
| postAttributeCollection | [identityApiConnector](identityapiconnector.md) | Указывает API, который будет вызываться после отправки пользователем собранных атрибутов и до создания пользователя во время регистрации.                                                      |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userFlowApiConnectorConfiguration"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowApiConnectorConfiguration"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "User flow API Connector Configuration",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: Resource userFlowApiConnectorConfiguration has documented navigation properties, but we thought it was a complex type!"
  ]
}-->
