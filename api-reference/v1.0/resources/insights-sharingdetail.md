---
title: тип ресурса sharingDetail
description: 'Сложный тип, содержащий свойства общих элементов. '
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 96840e801e7789c287dad26e014797013039a6a5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094291"
---
# <a name="sharingdetail-resource-type"></a>тип ресурса sharingDetail

Пространство имен: microsoft.graph

Сложный тип, содержащий свойства [элементов sharedInsight.](insights-shared.md) 

## <a name="json-representation"></a>Представление в формате JSON
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
| sharedDateTime        | DateTimeOffset| Дата и время последнего общего делиться файлом. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.  |
| sharingSubject        | Строка          | Тема, с которой был общий документ. |
| sharingType             | String        | Определяет способ общего делиться документом с помощью "Link", "Attachment", "Group", "Site".     |
| sharedBy                | [insightIdentity](insights-insightidentity.md)      | Пользователь, который поделился документом.  |
| sharingReference        | [resourceReference](insights-resourcereference.md)      |  |

