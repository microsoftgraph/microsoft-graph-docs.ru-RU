---
title: Тип ресурса programControlType
description: 'В Azure AD access дается обзор компонента, тип элемента управления программы используется, когда для связывания элемента управления в программу, чтобы указать тип доступа проверки элемента управления.  '
localization_priority: Normal
ms.openlocfilehash: 8b17a0f30fbdceb6b6da24d5cbe972223acb29b0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519705"
---
# <a name="programcontroltype-resource-type"></a>Тип ресурса programControlType

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD тип элемента управления программы используется при связывания элемента управления в программу, чтобы указать тип проверки доступа, управления.  

Объекты типа программа управления создаются автоматически при onboards глобального администратора клиента для использования доступа к дается обзор компонента.  Типы элементов управления не дополнительные программы могут быть созданы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список programControlTypes](../api/programcontroltype-list.md) | [programControlType](programcontroltype.md) коллекции| Список типов элементов управления программы. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| `id`                     |`String`                | Идентификатор компонента назначенные программы типа элемента управления                                      |
| `displayName`            |`String`                | Имя типа элемента управления программы                                                             |


## <a name="relationships"></a>Отношения

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

<!--
{
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/programcontroltype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
