---
title: Тип ресурса Програмконтролтипе
description: 'В функции рецензирования Access в Azure AD при сопоставлении элемента управления с программой используется тип элемента управления Program, чтобы указать тип проверки доступа, для которой предназначен элемент управления.  '
localization_priority: Normal
ms.openlocfilehash: 489fa6e5cac31165fec9f7ce9939d58fa84cb1ab
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344064"
---
# <a name="programcontroltype-resource-type"></a>Тип ресурса Програмконтролтипе

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции рецензирования [Access](accessreviews-root.md) в Azure AD при сопоставлении элемента управления с программой используется тип элемента управления Program, чтобы указать тип проверки доступа, для которой предназначен элемент управления.  

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


## <a name="relationships"></a>Связи

Отсутствуют.


## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание Програмконтрол](../api/programcontrol-create.md) |     [Програмконтрол](programcontrol.md) |   Добавление Програмконтрол в программу.|


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
