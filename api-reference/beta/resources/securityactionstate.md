---
title: Тип ресурса Секуритяктионстате
description: Представляет историю изменений состояния securityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 42037a6b65deb4bd3fc31d63c5cd47bee21b7eb7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520817"
---
# <a name="securityactionstate-resource-type"></a>Тип ресурса Секуритяктионстате

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет историю изменений состояния securityAction.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|appId|String|Идентификатор приложения вызывающего приложения, отправившего обновление (исправление) действию. Его `appId` необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением.|
|status|String| Состояние securityAction в этом обновлении. Возможные значения: `NotStarted`, `Running`, `Completed`, `Failed`.|
|упдатеддатетиме|DateTimeOffset| Временная метка при обновлении actionState. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|user|String|Имя участника-пользователя, который выполнил вход в действие при отправке обновления (исправления). Его `user` необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением.|

## <a name="json-representation"></a>Представление JSON

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
