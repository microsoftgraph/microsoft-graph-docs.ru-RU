---
title: Тип ресурса userFlowApiConnectorConfiguration
description: Представляет, какие соединители API включены для пользовательского потока.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 00b37f1b4bff0edf8aa85d79a01e23169b45dbcf
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720461"
---
# <a name="userflowapiconnectorconfiguration-resource-type"></a>Тип ресурса userFlowApiConnectorConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет, какие API-интерфейсы будут вызваны в определенных точках пользовательского потока.  Каждая связь этого объекта соответствует определенному шагу в пользовательском потоке, который можно настроить для вызова соединители API.

## <a name="relationships"></a>Отношения

| Связь            | Тип                                            | Описание                                                                                                                                             |
| :---------------------- | :---------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
| postFederationSignup    | [identityApiConnector](identityapiconnector.md) | Указывает API, который будет вызываться после федерации с внешним поставщиком удостоверений (например, Google, Facebook или Azure AD), после регистрации пользователя (не применяется для регистрации). |
| postAttributeCollection | [identityApiConnector](identityapiconnector.md) | Указывает API, который будет вызываться после отправки пользователем собранных атрибутов и до создания пользователя во время регистрации.                                                      |

## <a name="json-representation"></a>Представление JSON

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
