---
title: тип ресурса useDetails
description: Сложный тип, содержащий свойства используемых элементов. Сведения о том, когда последний доступ к ресурсу (просмотр) или изменение (редактирование) пользователем.
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3924577830b67733fd2e967fa9de4a30b1473492
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118539"
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
| lastAccessedDateTime                  | DateTimeOffset        | Дата и время последнего доступа пользователя к ресурсу. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.                     |
| lastModifiedDateTime              | DateTimeOffset        | Дата и время последнего изменения ресурса пользователем. Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, полночь UTC 1 января 2014 `2014-01-01T00:00:00Z` г. — это . Только для чтения.       |

