---
title: Тип ресурса Усерфлов
description: Пользовательские потоки идентификации — это встроенные пути проверки подлинности
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0d76d7a2ab3516717d01f0371b84531e211181fd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016639"
---
# <a name="userflow-resource-type"></a>Тип ресурса Усерфлов

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Потоки пользователей позволяют определить предопределенные настраиваемые политики для входа, регистрации, объединения и входа в систему, сброса пароля и обновления профиля.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/identityuserflow-list.md) | Коллекция [усерфлов](identityuserflow.md) | Список Усерфловс. |
| [создание](../api/identityuserflow-post-userflows.md); | [усерфлов](identityuserflow.md) | Создание объекта Усерфлов. |
| [получение](../api/identityuserflow-get.md); | [усерфлов](identityuserflow.md) | Чтение свойств и связей объекта Усерфлов. |
| [Удаление](../api/identityuserflow-delete.md) | Нет | Удаление объекта Усерфлов. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Только для чтения.|
|userFlowType|string| Возможные значения: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.|
|усерфловтипеверсион|Одинарное| Это версия пользовательского типа. Каждый тип пользовательского типа может иметь различные варианты, например 1, 1,1 или 2.  |

## <a name="relationships"></a>Отношения

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.UserFlow",
  "baseType": "",
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


