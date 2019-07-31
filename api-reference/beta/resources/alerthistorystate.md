---
title: Тип ресурса Алерсистористате
description: Сохраняет изменения, внесенные в оповещения.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 9467da6f5b088e9b1fadd3797a8b10f4b6e820db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974425"
---
# <a name="alerthistorystate-resource-type"></a>Тип ресурса Алерсистористате

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сохраняет изменения, внесенные в оповещения.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|appId|String| Идентификатор приложения для вызывающего приложения, отправившего обновление (исправление) в оповещение. AppId необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением. |
|assignedTo|String| UPN пользователя оповещение было назначено (Примечание: Alert. assignedTo содержит только Последнее значение/UPN). |
|comments|Коллекция String|Комментарий, введенный пользователем, который выполнил вход.|
|feedback|String| Обратная связь аналитика с оповещением в этом обновлении. Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.|
|status|Строка| Значение состояния оповещения (при обновлении). Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.|
|Упдатеддатетиме|DateTimeOffset| Дата и время обновления оповещения. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|user|String| UPN пользователя, выполнившего вход, который обновил оповещение (берется из маркера носителя — если в режиме пользователя или делегированной проверки подлинности). |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertHistoryState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "assignedTo": "String",
  "comments": ["String"],
  "feedback": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertHistoryState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->