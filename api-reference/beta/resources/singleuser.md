---
title: сложный тип SingleUser.
description: Определяет пользователя в клиенте, который будет разрешен в качестве запрашивающего, утверждающего или проверяющего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0d4db47278051dd79b697dc352549b95b872e4aa
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331406"
---
# <a name="singleuser-complex-type"></a>сложный тип SingleUser.

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в параметрах просмотра запроса, утверждения и назначения для [политики назначения пакетов Access](accesspackageassignmentpolicy.md). Это `@odata.type` значение `#microsoft.graph.singleUser` указывает на то, что этот набор пользователей определяет определенного пользователя в клиенте, который будет разрешен в качестве запрашивающего, утверждающего или проверяющего.

## <a name="properties"></a>Свойства

Этот тип имеет следующие свойства:

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| id |Строка | Идентификатор пользователя в Azure AD. |
| description |String | Имя пользователя в Azure AD. Только для чтения. |
| Создание резервной копии | Логический | Для **SingleUser.** на этапе утверждения указывает, является ли пользователь утверждающим резервной копии. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено представление типа в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singleUser",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false,
  "id": "string (identifier)",
  "description": "string"
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleUser complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
