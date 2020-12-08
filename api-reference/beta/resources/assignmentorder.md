---
title: Тип ресурса Ассигнментордер
description: Используется для определения порядка атрибутов, собранных в пользовательском движении.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 41b75e1adf5459279b5675278a8f00a82110b457
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581338"
---
# <a name="assignmentorder-resource-type"></a>Тип ресурса Ассигнментордер

Пространство имен: microsoft.graph

Используется для определения порядка атрибутов, собранных в пользовательском движении. Этот параметр определяет способ отображения страницы коллекции атрибутов, когда пользователь подписывается через пользовательский ход.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|порядке|Коллекция объектов string|Список идентификаторов Идентитюсерфловаттрибуте, предоставляемых для определения порядка, в котором атрибуты должны быть собраны в пользовательском цикле.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentOrder"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.assignmentOrder",
  "order": [
    "String"
  ]
}
```
