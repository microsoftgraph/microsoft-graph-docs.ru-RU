---
title: Тип ресурса Шарингдетаил
description: 'Сложный тип, содержащий свойства общих элементов. '
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4a2dc75ed2a62d7a67538bdef801bd97133fbd15
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333568"
---
# <a name="sharingdetail-resource-type"></a>Тип ресурса Шарингдетаил

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип, содержащий свойства [общих](insights-shared.md) элементов. 

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
| Шарингсубжект        | String          | Тема, к которой был предоставлен общий доступ к документу. |
| Шарингтипе             | String        | Определяет способ предоставления общего доступа к документу, который может быть "ссылка", "вложение", "Группа", "сайт".     |
| sharedBy                | [insightIdentity](insights-insightidentity.md)      | Пользователь, имеющий общий доступ к документу.  |
| Шарингреференце        | [Ресаурцереференце](insights-resourcereference.md)      |  |
