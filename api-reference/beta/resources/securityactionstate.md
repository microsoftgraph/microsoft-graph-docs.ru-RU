---
title: Тип ресурса Секуритяктионстате
description: Представляет историю изменений состояния securityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8f789dab438316f16b9c2607947fa08b7fcefdc2
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366933"
---
# <a name="securityactionstate-resource-type"></a>Тип ресурса Секуритяктионстате

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет историю изменений состояния securityAction.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|appId|String|Идентификатор приложения вызывающего приложения, отправившего обновление (исправление) действию. Его `appId` необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением.|
|status|Строка| Состояние securityAction в этом обновлении. Возможные значения: `NotStarted`, `Running`, `Completed`, `Failed`.|
|Упдатеддатетиме|DateTimeOffset| Временная метка при обновлении actionState. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|user|String|Имя участника-пользователя, который выполнил вход в действие при отправке обновления (исправления). Его `user` необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением.|

## <a name="json-representation"></a>Описание в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityActionState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityActionState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
