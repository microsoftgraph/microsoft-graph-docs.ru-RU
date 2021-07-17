---
title: тип ресурса connectionOperation
description: Описывает состояние асинхронного запроса для создания схемы Поиск (Майкрософт) подключения.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1b9e3bf811807213970694ebe4e7748bf59e32ef
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467828"
---
# <a name="connectionoperation-resource-type"></a>тип ресурса connectionOperation

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает состояние асинхронного запроса для создания схемы Поиск (Майкрософт) [подключения.](externalconnectors-schema.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Get connectionOperation](../api/externalconnectors-connectionoperation-get.md) | [connectionOperation](externalconnectors-connectionoperation.md) | Чтение свойств объекта connectionOperation. |

## <a name="properties"></a>Свойства

| Свойство | Тип                          | Описание                       |
|:---------|:------------------------------|:----------------------------------|
| error    | [publicError](publicerror.md) | Если `status` это `failed` так, предоставляет дополнительные сведения об ошибке, которая привела к сбою. |
| id       | String                        | Уникальный идентификатор для подключенияOperation. Только для чтения. |
| status   | String                        | Указывает состояние асинхронной операции. Возможные значения: `unspecified`, `inprogress`, `completed`, `failed`. |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.connectionOperation",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectionOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
