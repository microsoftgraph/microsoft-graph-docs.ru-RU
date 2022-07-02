---
title: Тип ресурса deletedTeam
description: Это удаленная команда в Microsoft Teams.
author: agnesliu
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: de027a7e224db03f72fe424c1a4e08f5d238bea7
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2022
ms.locfileid: "66578142"
---
# <a name="deletedteam-resource-type"></a>Тип ресурса deletedTeam

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Это удаленная [команда](../resources/team.md) в Microsoft Teams.

Каждая удаленная команда связана с [группой Microsoft 365](../resources/group.md). Дополнительные сведения о работе с группами и участниками в командах см. в статье [Использование интерфейса API Microsoft Graph для работы с Microsoft Teams](teams-api-overview.md).

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[getAllMessages](../api/deletedteam-getallmessages.md)|Коллекция [chatMessage](../resources/chatmessage.md)|Извлечение всех [сообщений](../resources/chatmessage.md) из всех [каналов](../resources/channel.md) в [удаленной команде](../resources/deletedteam.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор удаленной команды. Наследуется от [сущности](../resources/entity.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|channels|Коллекция [channel](../resources/channel.md)|Каналы, используемые вместе с удаленной командой или создаваемые в удаленной команде.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deletedTeam",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
    "@odata.type": "#microsoft.graph.deletedTeam",
    "id": "String (identifier)"
}
```

