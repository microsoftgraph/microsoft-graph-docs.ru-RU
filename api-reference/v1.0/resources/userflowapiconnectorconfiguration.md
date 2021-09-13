---
title: тип ресурса userFlowApiConnectorConfiguration
description: Представляет соединители API, которые включены для потока пользователей.
author: nickgmicrosoft
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2f58a1d64d863ab09fdd5713a0f41b5143cb5630
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59083945"
---
# <a name="userflowapiconnectorconfiguration-resource-type"></a>тип ресурса userFlowApiConnectorConfiguration

Пространство имен: microsoft.graph

Определяет API, которые называются в определенных точках пользовательского потока.  Каждое отношение этого объекта соответствует определенному шагу в потоке пользователей, который можно настроить для вызова соединиттеля API.

## <a name="relationships"></a>Отношения

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
