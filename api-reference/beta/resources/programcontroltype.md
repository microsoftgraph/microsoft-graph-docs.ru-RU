---
title: Тип ресурса programControlType
description: 'В Azure AD access дается обзор компонента, тип элемента управления программы используется, когда для связывания элемента управления в программу, чтобы указать тип доступа проверки элемента управления.  '
ms.openlocfilehash: 8fc406648d8f8c943920507a5734f47d2add1b4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078790"
---
# <a name="programcontroltype-resource-type"></a>Тип ресурса programControlType

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD тип элемента управления программы используется при связывания элемента управления в программу, чтобы указать тип проверки доступа, управления.  

Объекты типа программа управления создаются автоматически при onboards глобального администратора клиента для использования доступа к дается обзор компонента.  Типы элементов управления не дополнительные программы могут быть созданы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список programControlTypes](../api/programcontroltype-list.md) | [programControlType](programcontroltype.md) коллекции| Список типов элементов управления программы. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
| `id`                     |`String`                | Идентификатор компонента назначенные программы типа элемента управления                                      |
| `displayName`            |`String`                | Имя типа элемента управления программы                                                             |


## <a name="relationships"></a>Связи

Нет.


## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Добавьте programControl программы.|


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

<!-- {
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
