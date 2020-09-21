---
title: сложный тип SingleUser.
description: Определяет пользователя в клиенте, который будет разрешен в качестве запрашивающего, утверждающего или проверяющего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fb6b665814281629836f4c5148b567de776ef2ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067127"
---
# <a name="singleuser-complex-type"></a>сложный тип SingleUser.

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в параметрах просмотра запроса, утверждения и назначения для [политики назначения пакетов Access](accesspackageassignmentpolicy.md). `@odata.type`Это значение `#microsoft.graph.singleUser` указывает на то, что этот набор пользователей определяет определенного пользователя в клиенте, который будет разрешен в качестве запрашивающего, утверждающего или проверяющего.

## <a name="properties"></a>Свойства

Этот тип имеет следующие свойства:

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| id |String | Идентификатор пользователя в Azure AD. |
| description |String | Имя пользователя в Azure AD. Только для чтения. |
| Создание резервной копии | Boolean | Для **SingleUser.** на этапе утверждения указывает, является ли пользователь утверждающим резервной копии. |

## <a name="json-representation"></a>Представление в формате JSON

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


