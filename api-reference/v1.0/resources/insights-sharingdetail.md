---
title: тип ресурса sharingDetail
description: 'Сложный тип, содержащий свойства общих элементов. '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 341bef801b8ee8a7cfc8b5176f4984251209db9e4aff05de9d983b8e06cb61fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124467"
---
# <a name="sharingdetail-resource-type"></a>тип ресурса sharingDetail

Пространство имен: microsoft.graph

Сложный тип, содержащий свойства [элементов sharedInsight.](insights-shared.md) 

## <a name="json-representation"></a>Представление JSON
Ниже показано представление JSON ресурса.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingDetail"
}-->
```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "sharingReference": "resourceReference"
}
```

## <a name="properties"></a>Свойства

| Свойство              | Тип          | Описание  |
| -------------         |-----------    | -------------|
| sharedDateTime        | DateTimeOffset| Дата и время последнего общего делиться файлом. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`. Только для чтения.  |
| sharingSubject        | String          | Тема, с которой был общий документ. |
| sharingType             | String        | Определяет способ общего делиться документом с помощью "Link", "Attachment", "Group", "Site".     |
| sharedBy                | [insightIdentity](insights-insightidentity.md)      | Пользователь, который поделился документом.  |
| sharingReference        | [resourceReference](insights-resourcereference.md)      |  |

