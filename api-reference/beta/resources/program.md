---
title: тип ресурса программы (не рекомендуется)
description: 'В Azure AD проверки доступа программа представляет собой контейнер, содержащий элементы управления программой. Клиент может иметь одну или несколько программ.  Каждый элемент управления связывает проверку доступа с программой, чтобы упростить поиск связанных проверок доступа.  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: f0d0a7a42a21a95bbf57b971d09e20046bd46ffa
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819400"
---
# <a name="program-resource-type-deprecated"></a>тип ресурса программы (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

В Azure AD [проверки доступа](accessreviews-root.md) программа представляет собой контейнер, содержащий элементы управления программой. Клиент может иметь одну или несколько программ.  Каждый элемент управления связывает проверку доступа с программой, чтобы упростить поиск связанных проверок доступа.  

Каждый клиент, в котором есть Azure AD проверки доступа, имеет одну программу. `Default program`  Глобальный администратор может создавать дополнительные программы, например для представления инициатив по соответствию требованиям. 


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание программы](../api/program-create.md) |   [Программа](program.md)   |   Создайте новую программу.|
|[Удаление программы](../api/program-delete.md) |   Нет.   |   Удалите программу.|
|[Перечисление программ](../api/program-list.md) |  [коллекция программ](program.md)|   Получение коллекции всех программ.|
|[Перечисление programControls программы](../api/program-listcontrols.md) |      [Коллекция programControl](programcontrol.md)| Получение коллекции элементов управления программы.|
|[Обновление программы](../api/program-update.md) |   [Программа](program.md)|  Обновление программы.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| id                        |Строка                              |  Идентификатор программы, назначаемой компонентом.                    |
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


