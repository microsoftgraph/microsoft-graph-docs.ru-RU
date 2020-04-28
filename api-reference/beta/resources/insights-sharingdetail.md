---
title: Тип ресурса Шарингдетаил
description: 'Сложный тип, содержащий свойства общих элементов. '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: e8216e08c4f7232c67c51fa8291ece63178472b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495601"
---
# <a name="sharingdetail-resource-type"></a>Тип ресурса Шарингдетаил

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип, содержащий свойства элементов [шарединсигхт](insights-shared.md) . 

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
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a>Свойства

| Свойство              | Тип          | Описание  |
| -------------         |-----------    | -------------|
| sharedDateTime        | DateTimeOffset| Дата и время последнего предоставления общего доступа к файлу. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`. Только для чтения.  |
| шарингсубжект        | String          | Тема, к которой был предоставлен общий доступ к документу. |
| шарингтипе             | String        | Определяет способ предоставления общего доступа к документу, который может быть "ссылка", "вложение", "Группа", "сайт".     |
| sharedBy                | [insightIdentity](insights-insightidentity.md)      | Пользователь, имеющий общий доступ к документу.  |
| шарингреференце        | [ресаурцереференце](insights-resourcereference.md)      |  |
