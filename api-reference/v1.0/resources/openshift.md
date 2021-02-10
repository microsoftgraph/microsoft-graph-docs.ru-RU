---
title: Тип ресурса openShift
description: Представляет неназначить открытую смену в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9d513c73cebdc2cc039f53c395c6ff7c1411f806
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158690"
---
# <a name="openshift-resource-type"></a>Тип ресурса openShift

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет неназначить открытую смену в [расписании.](../resources/schedule.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/openshift-list.md) | Коллекция [openShift](openshift.md) | Список свойств и связей объектов **openShift** в команде.|
| [Создание](../api/openshift-post.md) | [openShift](openshift.md) | Создание экземпляра объекта **openShift.** |
| [Получение](../api/openshift-get.md) | [openShift](openshift.md) | Чтение свойств и связей объекта **openShift.** |
| [Обновление](../api/openshift-update.md) | [openShift](openshift.md) | Обновление объекта **openShift.** |
| [удаление](../api/openshift-delete.md); | Нет | Удаление объекта **openShift.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|draftOpenShift|[openShiftItem](openshiftitem.md)|Неопубликоваемая открытая смена.|
|schedulingGroupId|String|ИД группы планирования, к которой принадлежит открытая смена.|
|sharedOpenShift|[openShiftItem](openshiftitem.md)|Опубликованная открытая смена.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShift"
}-->

```json
{
  "draftOpenShift": {"@odata.type": "microsoft.graph.openShiftItem"},
  "schedulingGroupId": "String",
  "sharedOpenShift": {"@odata.type": "microsoft.graph.openShiftItem"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

