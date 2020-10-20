---
title: Тип ресурса Програмресаурце
description: Представляет ссылку на объект, который является целевым объектом проверки доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5ad3720587523e6937b4c3713a1c5a8c06d1e6e5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601498"
---
# <a name="programresource-resource-type"></a>Тип ресурса Програмресаурце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект **програмресаурце** , содержащийся в объекте [програмконтрол](programcontrol.md) , представляет ссылку на объект, который является целевым объектом проверки доступа.

Этот тип наследуется от [Identity](identity.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| type | String | Тип ресурса, указывающий, является ли он группой или приложением. |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.programResource"
}-->
```json
{
  "type": "string"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "programResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
