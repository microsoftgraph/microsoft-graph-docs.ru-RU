---
title: тип ресурса programControlType
description: 'В функции обзоров доступа Azure AD используется тип управления программой при присоединении элементов управления к программе, чтобы указать тип обзора доступа, для который используется элемент управления.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 58c9ee3ade6e3969de9653f54c5181a66f087ea5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960364"
---
# <a name="programcontroltype-resource-type"></a>тип ресурса programControlType

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции обзоров доступа Azure [AD](accessreviews-root.md) используется тип управления программой при присоединении элементов управления к программе, чтобы указать тип обзора доступа, для который используется элемент управления.  

Объекты типа управления программами автоматически создаются, когда глобальный администратор на борту клиента использует функцию обзоров доступа.  Дополнительные типы управления программами не создаются.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[List programControlTypes](../api/programcontroltype-list.md) | [коллекция programControlType](programcontroltype.md)| Типы управления программами списка. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| id                     |Строка                | Идентификатор типа управления программой, заданная функцией                                      |
| displayName            |Строка                | Имя типа управления программой                                                             |


## <a name="relationships"></a>Связи

Отсутствуют.


## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Добавьте программуControl в программу.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControlType"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


