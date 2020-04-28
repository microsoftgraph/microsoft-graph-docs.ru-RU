---
title: Тип ресурса Усерфлов
description: Пользовательские потоки идентификации — это встроенные пути проверки подлинности
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d14722844c6449a585ca023df80fccb4e9d7c90b
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218459"
---
# <a name="userflow-resource-type"></a>Тип ресурса Усерфлов

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Потоки пользователей позволяют определить предопределенные настраиваемые политики для входа, регистрации, объединения и входа в систему, сброса пароля и обновления профиля.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [List](../api/identityuserflow-list.md) | Коллекция [усерфлов](identityuserflow.md) | Список Усерфловс. |
| [создание](../api/identityuserflow-post-userflows.md); | [усерфлов](identityuserflow.md) | Создание объекта Усерфлов. |
| [получение](../api/identityuserflow-get.md); | [усерфлов](identityuserflow.md) | Чтение свойств и связей объекта Усерфлов. |
| [удаление](../api/identityuserflow-delete.md); | Нет | Удаление объекта Усерфлов. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Только для чтения.|
|усерфловтипе|string| Возможные значения: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.|
|усерфловтипеверсион|Одинарное| Это версия пользовательского типа. Каждый тип пользовательского типа может иметь различные варианты, например 1, 1,1 или 2.  |

## <a name="relationships"></a>Связи

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
