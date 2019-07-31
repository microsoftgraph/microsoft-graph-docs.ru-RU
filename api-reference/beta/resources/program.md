---
title: Тип ресурса Program
description: 'В функции рецензирования Access в Azure AD программа — это контейнер, содержащий программные элементы управления. У клиента может быть одна или несколько программ.  Каждый элемент управления содержит ссылку на проверку доступа к программе, чтобы упростить обнаружение связанных проверок доступа.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c6a978ef4bb68c09b2f5659e255d16681c9c805d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965672"
---
# <a name="program-resource-type"></a>Тип ресурса Program

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции рецензирования [Access](accessreviews-root.md) в Azure AD программа — это контейнер, содержащий программные элементы управления. У клиента может быть одна или несколько программ.  Каждый элемент управления содержит ссылку на проверку доступа к программе, чтобы упростить обнаружение связанных проверок доступа.  

У каждого клиента, у которого есть встроенные обзоры Azure AD, есть одна программа `Default program`.  Глобальный администратор может создавать дополнительные программы, например для представления инициатив по обеспечению соответствия требованиям. 


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание программы](../api/program-create.md) |   [Программа](program.md)   |   Создайте новую программу.|
|[Удаление программы](../api/program-delete.md) |   Нет.   |   Удаление программы.|
|[Список программ](../api/program-list.md) |  Коллекция [Program](program.md)|   Получение коллекции всех программ.|
|[Список Програмконтролс программы](../api/program-listcontrols.md) |      Коллекция [програмконтрол](programcontrol.md)| Получение коллекции элементов управления программы.|
|[Программа обновления](../api/program-update.md) |   [Программа](program.md)|  Обновление программы.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  Идентификатор программы, назначенный компонентом.                    |
| `displayName`               |`String`                              |  Имя программы.  Требуется при создании.                  |
| `description`               |`String`                              |  Описание программы.           |

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
| `controls`                  |[Програмконтрол](programcontrol.md) | Элементы управления, связанные с программой. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.program"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "description": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
