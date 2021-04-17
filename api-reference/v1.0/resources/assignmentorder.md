---
title: тип ресурса assignmentOrder
description: Определяет порядок атрибутов, собираемого в потоке пользователей.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4c5faed250c07d5c4416c91a5452f1276c6b728e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883061"
---
# <a name="assignmentorder-resource-type"></a>тип ресурса assignmentOrder

Пространство имен: microsoft.graph

Используется для определения порядка атрибутов, собираемого в потоке пользователей. Порядок определяет отображение страницы коллекции атрибутов при записи пользователя с помощью пользовательского потока.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|порядок|Коллекция строк|Список идентификаторов объектов identityUserFlowAttribute, определяющих порядок сбора атрибутов в потоке пользователей.|

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
