---
title: Тип ресурса Теамстемплате
description: Описывает объект Теамстемплате.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ba27dc19f1d6561784d26105bcf8e089c664bbf1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088442"
---
# <a name="teamstemplate-resource-type"></a>Тип ресурса Теамстемплате

Пространство имен: microsoft.graph

Шаблон группы — это план для создания [команды](../resources/team.md) в Microsoft Teams. Шаблон определяет структуру, параметры и даже содержимое, которое должно быть подготовлено в новой команде, созданной с помощью шаблона. Корпорация Майкрософт предоставляет набор базовых шаблонов и клиентов, которые могут сохранять собственные настраиваемые шаблоны.

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | Строка   | Уникальный идентификатор шаблона. Не может иметь значение null. |

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

## <a name="see-also"></a>См. также

- [team](team.md)


