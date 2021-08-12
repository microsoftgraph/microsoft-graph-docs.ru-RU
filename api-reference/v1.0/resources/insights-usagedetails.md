---
title: тип ресурса useDetails
description: Сложный тип, содержащий свойства используемых элементов. Сведения о том, когда последний доступ к ресурсу (просмотр) или изменение (редактирование) пользователем.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 1fe25cc2bab141b3ac29e47b4bca80d8dc24fbe7be410be32398475c9e9a7d14
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54216842"
---
# <a name="usagedetails-resource-type"></a>тип ресурса useDetails

Пространство имен: microsoft.graph

Сложный тип, содержащий свойства [используемых](insights-used.md) элементов. Сведения о том, когда последний доступ к ресурсу (просмотр) или изменение (редактирование) пользователем.


## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.usageDetails"
}-->

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a>Свойства

| Свойство              | Тип          | Описание  |
| -------------         |---------------| -------------|
| lastAccessedDateTime                  | DateTimeOffset        | Дата и время последнего доступа пользователя к ресурсу. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`. Только для чтения.                      |
| lastModifiedDateTime              | DateTimeOffset        | Дата и время последнего изменения ресурса пользователем. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`. Только для чтения.       |

