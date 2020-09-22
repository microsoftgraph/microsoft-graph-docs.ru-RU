---
title: Тип ресурса Алерсистористате
description: Сохраняет изменения, внесенные в оповещения.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: cf8043b4409b29220841e2706649050003b09f34
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004286"
---
# <a name="alerthistorystate-resource-type"></a>Тип ресурса Алерсистористате

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сохраняет изменения, внесенные в оповещения.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|appId|String| Идентификатор приложения для вызывающего приложения, отправившего обновление (исправление) в оповещение. AppId необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением. |
|assignedTo|String| UPN пользователя оповещение было назначено (Примечание: Alert. assignedTo содержит только Последнее значение/UPN). |
|comments|Коллекция String|Комментарий, введенный пользователем, который выполнил вход.|
|feedback|String| Обратная связь аналитика с оповещением в этом обновлении. Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.|
|status|String| Значение состояния оповещения (при обновлении). Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.|
|упдатеддатетиме|DateTimeOffset| Дата и время обновления оповещения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
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

