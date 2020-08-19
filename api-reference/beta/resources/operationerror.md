---
title: Тип ресурса Оператионеррор
description: Описание ошибок в Теамсасинкоператион.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: billbliss
ms.openlocfilehash: 2419d4230e5618f601a5d8fe0743ec9ef807cf00
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809329"
---
# <a name="operationerror-resource-type"></a>Тип ресурса Оператионеррор

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описание ошибок в [теамсасинкоператион](teamsasyncoperation.md).

## <a name="operationerror-properties"></a>Свойства Оператионеррор
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|code|string (только для чтения)|Код ошибки операции.|
|message|string (только для чтения)|Сообщение об ошибке операции.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
