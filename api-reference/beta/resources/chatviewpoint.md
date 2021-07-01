---
title: тип ресурса chatViewpoint
description: Представляет пользовательские свойства чата.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca6a542903aae7b203c6183a25dd99889b97f275
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236327"
---
# <a name="chatviewpoint-resource-type"></a>тип ресурса chatViewpoint

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользовательские свойства [чата.](../resources/chat.md) Эти свойства могут изменяться в зависимости от того, кто является звонивцом API.

> **Примечание:** В настоящее время [только операция чатов](../api/chat-list.md) списка поддерживает **chatViewpoint.**

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastMessageReadDateTime|DateTimeOffset|Представляет dateTime до тех пор, пока пользователь звонка не прочитал [chatMessages в](../resources/chatmessage.md) определенном чате.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatViewpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatViewpoint",
  "lastMessageReadDateTime": "String (timestamp)"
}
```

