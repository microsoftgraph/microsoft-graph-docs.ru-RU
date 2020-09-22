---
title: Тип ресурса Програмконтролтипе
description: 'В функции рецензирования Access в Azure AD при сопоставлении элемента управления с программой используется тип элемента управления Program, чтобы указать тип проверки доступа, для которой предназначен элемент управления.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: ddf5ee29c01770d06c9725413f362bd0f0e18bee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029066"
---
# <a name="programcontroltype-resource-type"></a>Тип ресурса Програмконтролтипе

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции [рецензирования Access](accessreviews-root.md) в Azure AD при сопоставлении элемента управления с программой используется тип элемента управления Program, чтобы указать тип проверки доступа, для которой предназначен элемент управления.  

Объекты типа управления программой автоматически создаются, когда глобальный администратор, входящей в клиент, должен использовать функцию "обзоры доступа".  Невозможно создать дополнительные типы элементов управления программы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список Програмконтролтипес](../api/programcontroltype-list.md) | Коллекция [програмконтролтипе](programcontroltype.md)| Список типов элементов управления программы. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| `id`                     |`String`                | Идентификатор типа программного элемента управления, назначенный с помощью функции                                      |
| `displayName`            |`String`                | Имя типа элемента управления программы                                                             |


## <a name="relationships"></a>Отношения

Отсутствуют.


## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание Програмконтрол](../api/programcontrol-create.md) |     [програмконтрол](programcontrol.md) |   Добавление Програмконтрол в программу.|


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


