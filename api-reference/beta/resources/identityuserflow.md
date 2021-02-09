---
title: Тип ресурса UserFlow
description: Потоки пользователей удостоверений — это встроенные пути проверки подлинности
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4b4842b506e3c3c3e675ec2a47837fbf0c2e10be
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158291"
---
# <a name="userflow-resource-type"></a>Тип ресурса UserFlow

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Потоки пользователей позволяют определять предварительно определенные настраиваемые политики для входов, регистрации, объединенной регистрации и входов, сброса паролей и обновления профиля.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/identityuserflow-list.md) | [Коллекция UserFlow](identityuserflow.md) | Список userFlows. |
| [Создание](../api/identityuserflow-post-userflows.md) | [UserFlow](identityuserflow.md) | Создание объекта UserFlow. |
| [Получение](../api/identityuserflow-get.md) | [UserFlow](identityuserflow.md) | Чтение свойств и связей объекта UserFlow. |
| [удаление](../api/identityuserflow-delete.md); | Нет | Удаление объекта UserFlow. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Только для чтения.|
|userFlowType|string| Возможные значения: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.|
|userFlowTypeVersion|Одинарное| Это версия типа пользовательского потока. Каждый тип пользовательского потока может иметь различные возможные версии, например 1, 1.1 или 2.  |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.UserFlow",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "userFlowType": "string",
  "userFlowTypeVersion": "Single"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UserFlow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


