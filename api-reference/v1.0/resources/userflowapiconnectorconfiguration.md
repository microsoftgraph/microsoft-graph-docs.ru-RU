---
title: тип ресурса userFlowApiConnectorConfiguration
description: Представляет соединители API, которые включены для потока пользователей.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 474011cceb4c05e2c1b8f61aa4ea0e05e03df26857a0c10ea3a7197d453d24c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230419"
---
# <a name="userflowapiconnectorconfiguration-resource-type"></a>тип ресурса userFlowApiConnectorConfiguration

Пространство имен: microsoft.graph

Определяет API, которые называются в определенных точках пользовательского потока.  Каждое отношение этого объекта соответствует определенному шагу в потоке пользователей, который можно настроить для вызова соединиттеля API.

## <a name="relationships"></a>Связи

| Связь            | Тип                                            | Описание                                                                                                                                             |
| :---------------------- | :---------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
| postFederationSignup    | [identityApiConnector](identityapiconnector.md) | Указывает API для вызова федерации с внешним поставщиком удостоверений. Например, API Google, Facebook или Azure AD завершится при регистрации пользователя (не применяется к входу). |
| postAttributeCollection | [identityApiConnector](identityapiconnector.md) | Указывает API для вызова после отправки пользователем собранных атрибутов и до создания учетной записи пользователя во время регистрации.                                                      |

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
  ]
}-->
