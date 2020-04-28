---
title: Тип ресурса Теамстемплате
description: Описывает объект Теамстемплате.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 77101c756e09b4ce2356da2384f2c50b119ae856
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519836"
---
# <a name="teamstemplate-resource-type"></a>Тип ресурса Теамстемплате

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Шаблон группы — это план для создания [команды](../resources/team.md) в Microsoft Teams. Шаблон определяет структуру, параметры и даже содержимое, которое должно быть подготовлено в новой команде, созданной с помощью шаблона. Корпорация Майкрософт предоставляет набор базовых шаблонов и клиентов, которые могут сохранять собственные настраиваемые шаблоны.

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | String   | Уникальный идентификатор шаблона. Не может иметь значение null. |

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a>См. также

- [team](team.md)

