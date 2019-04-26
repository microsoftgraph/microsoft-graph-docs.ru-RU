---
title: Тип ресурса Алерсистористате
description: Сохраняет изменения, внесенные в оповещения.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 1a7975d870389be5163a8f230f6a6cc4cd1425c3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339158"
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
|замечания|String| Обратная связь аналитика с оповещением в этом обновлении. Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.|
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