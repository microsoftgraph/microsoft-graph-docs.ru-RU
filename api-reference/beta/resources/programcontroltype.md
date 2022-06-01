---
title: Тип ресурса programControlType (не рекомендуется)
description: 'В Azure AD проверки доступа тип управления программой используется при связывание элемента управления с программой, чтобы указать тип проверки доступа, для который предназначен элемент управления.  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 2dcb4c5e00b4c3b5ea0cf9283dadaa9b2c89cd12
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819743"
---
# <a name="programcontroltype-resource-type-deprecated"></a>Тип ресурса programControlType (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

В Azure AD проверки доступа тип [](accessreviews-root.md) управления программой используется при связывание элемента управления с программой, чтобы указать тип проверки доступа, для который предназначен элемент управления.  

Объекты типов программных элементов управления создаются автоматически, когда глобальный администратор подключает клиент для использования функции проверки доступа.  Дополнительные типы элементов управления программой создаваться не могут.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление programControlTypes](../api/programcontroltype-list.md) | [Коллекция programControlType](programcontroltype.md)| Перечисление типов элементов управления программой. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| id                     |Строка                | Назначенный функцией идентификатор типа элемента управления программы                                      |
| displayName            |Строка                | Имя типа элемента управления программы                                                             |


## <a name="relationships"></a>Связи

Отсутствуют.


## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание объекта programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Добавьте programControl в программу.|


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


