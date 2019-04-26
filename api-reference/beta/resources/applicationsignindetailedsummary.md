---
title: Тип ресурса Аппликатионсигниндетаиледсуммари — API Microsoft Graph
description: Представляет подробные сведения о входе в приложение.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 783201ec40ac0749d2c2999649bf1c420eaba5b6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328530"
---
# <a name="applicationsignindetailedsummary-resource-type"></a>Тип ресурса Аппликатионсигниндетаиледсуммари

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения о входе в приложение.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение Аппликатионсигниндетаиледсуммари](../api/applicationsignindetailedsummary-get.md) | [Аппликатионсигниндетаиледсуммари](applicationsignindetailedsummary.md) | Чтение свойств и связей объекта **аппликатионсигниндетаиледсуммари** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|Аггрегатедевентдатетиме|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|appDisplayName|String|Имя приложения, в которое пользователь выполнил вход.|
|appId|String|Идентификатор приложения, в который пользователь выполнил вход.|
|id|Строка| Уникальный идентификатор, представляющий действия при входе.|
|Сигнинкаунт|Int64|Количество входов, выполненных приложением.|
|status|[signInStatus](signinstatus.md)|Сведения о состоянии входа.|

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationSignInDetailedSummary"
}-->

```json
{
  "aggregatedEventDateTime": "String (timestamp)",
  "appDisplayName": "String",
  "appId": "String",
  "id": "String (identifier)",
  "signInCount": 1024,
  "status": {"@odata.type": "microsoft.graph.signInStatus"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationSignInDetailedSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
