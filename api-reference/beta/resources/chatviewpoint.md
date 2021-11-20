---
title: тип ресурса chatViewpoint
description: Представляет пользовательские свойства чата.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9d9efb70dec447bf2f3c504a05245f67944783f6
ms.sourcegitcommit: 70b3caded085ba8ef15e389f81fa005506f1e2fb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2021
ms.locfileid: "61131926"
---
# <a name="chatviewpoint-resource-type"></a>тип ресурса chatViewpoint

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользовательские свойства [чата.](../resources/chat.md) Эти свойства могут изменяться в зависимости от того, кто является звонивцом API.

> **Примечание:** В настоящее время [только операция чатов Списка](../api/chat-list.md) поддерживает **chatViewpoint.**

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isHidden|Логический|Указывает, скрыт ли чат для текущего пользователя.|
|lastMessageReadDateTime|DateTimeOffset|Представляет dateTime до тех пор, пока текущий пользователь не прочитал [chatMessages в](../resources/chatmessage.md) определенном чате.|

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
  "isHidden": "Boolean",
  "lastMessageReadDateTime": "String (timestamp)"
}
```

