---
title: Тип ресурса UserFlow
description: Потоки пользователей удостоверений — это встроенные пути проверки подлинности
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c5401aeb67ccc894e2c151507c0a857b14c3dabb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957025"
---
# <a name="userflow-resource-type"></a>Тип ресурса UserFlow

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Потоки пользователей позволяют определять заранее настроенные политики для регистрации, регистрации, комбинированной регистрации и регистрации, сброса паролей и обновления профиля.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/identityuserflow-list.md) | [Коллекция UserFlow](identityuserflow.md) | Список пользовательских процессов. |
| [Создание](../api/identityuserflow-post-userflows.md) | [UserFlow](identityuserflow.md) | Создание объекта UserFlow. |
| [получение](../api/identityuserflow-get.md); | [UserFlow](identityuserflow.md) | Чтение свойств и связей объекта UserFlow. |
| [удаление](../api/identityuserflow-delete.md); | Нет | Удаление объекта UserFlow. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка| Идентификатор потока пользователей. Префикс **B2C_1_** добавляется к предоставляемой вами стоимости.|
|userFlowType|userFlowType| Возможные значения: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.|
|userFlowTypeVersion|Одинарное| Это версия типа потока пользователя. Каждый тип потока пользователей может иметь различные возможные версии, такие как 1, 1.1 или 2.  |

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


