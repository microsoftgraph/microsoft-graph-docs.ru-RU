---
title: Тип ресурса Фрибусеррор
description: Представляет сведения об ошибке при попытке получить доступ к пользователю, списку рассылки или ресурсу.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: harini84
ms.openlocfilehash: e259685415a37e89429b5e0522e89a4fbe2f9fd2
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809539"
---
# <a name="freebusyerror-resource-type"></a>Тип ресурса Фрибусеррор

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об ошибке при попытке получить доступ к пользователю, списку рассылки или ресурсу.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|message |String |Описание ошибки. |
|респонсекоде |String |Код ответа из запроса на доступность пользователя, списка рассылки или ресурса. |


## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.freeBusyError"
}-->

```json
{
  "message": "String",
  "responseCode": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
