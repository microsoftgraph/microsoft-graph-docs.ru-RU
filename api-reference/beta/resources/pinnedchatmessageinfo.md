---
title: Тип ресурса pinnedChatMessageInfo
description: Представляет отдельное закрепленное сообщение в сущности чата.
author: sumanac
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d9ee744cfe71a2c9a8c05b0a8ed86c046827428d
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653660"
---
# <a name="pinnedchatmessageinfo-resource-type"></a>Тип ресурса pinnedChatMessageInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отдельное закрепленное сообщение в [чате](chat.md).


Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Вывод списка закрепленных сообщений в чате](../api/chat-list-pinnedmessages.md)|[Коллекция pinnedChatMessageInfo](../resources/pinnedchatmessageinfo.md)|Получение списка закрепленных сообщений в чате.|
|[Закрепление сообщения в чате](../api/chat-post-pinnedmessages.md)|[pinnedChatMessageInfo](../resources/pinnedchatmessageinfo.md)|Закрепите сообщение чата в чате.|
|[Открепление сообщения из чата](../api/chat-delete-pinnedmessages.md)|Нет|Открепите сообщение из чата.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| id| String| Идентификатор объекта [chatMessage](../resources/chatmessage.md). Только для чтения. |

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
| message | [chatMessage](../resources/chatmessage.md) | Представляет сведения о закрепленных сообщениях чата.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.pinnedChatMessageInfo",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.pinnedChatMessageInfo",
  "id": "String (identifier)"
}
```

