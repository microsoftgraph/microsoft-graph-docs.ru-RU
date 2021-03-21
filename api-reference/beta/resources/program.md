---
title: Тип ресурса программы
description: 'В функции обзоров доступа Azure AD программа является контейнером с элементом управления программой. Клиент может иметь одну или несколько программ.  Каждый контроль связывает обзор доступа с программой, чтобы упростить поиск соответствующих отзывов доступа.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: eb04c1e05c669758e282aebdcccfa4e55507e659
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960373"
---
# <a name="program-resource-type"></a>Тип ресурса программы

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции обзоров доступа Azure [AD](accessreviews-root.md) программа является контейнером с элементом управления программой. Клиент может иметь одну или несколько программ.  Каждый контроль связывает обзор доступа с программой, чтобы упростить поиск соответствующих отзывов доступа.  

Каждый клиент, у которых есть отзывы о доступе к Azure AD на борту, имеет одну программу. `Default program`  Глобальный администратор может создавать дополнительные программы, например для представления инициатив по обеспечению соответствия требованиям. 


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание программы](../api/program-create.md) |   [программа](program.md)   |   Создание новой программы.|
|[Удаление программы](../api/program-delete.md) |   Отсутствуют.   |   Удаление программы.|
|[Списки программ](../api/program-list.md) |  [коллекция](program.md) программ|   Получите коллекцию всех программ.|
|[Список программКонтроли программы](../api/program-listcontrols.md) |      [коллекция programControl](programcontrol.md)| Получите коллекцию элементов управления программы.|
|[Программа обновления](../api/program-update.md) |   [программа](program.md)|  Обновление программы.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| id                        |Строка                              |  Идентификатор программы, заданная функцией.                    |
| displayName               |Строка                              |  Имя программы.  Требуется при создании.                  |
| description               |Строка                              |  Описание программы.           |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| `controls`                  |[programControl](programcontrol.md) | Элементы управления, связанные с программой. |

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


