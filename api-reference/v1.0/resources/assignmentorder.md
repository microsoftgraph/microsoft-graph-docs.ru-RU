---
title: тип ресурса assignmentOrder
description: Определяет порядок атрибутов, собираемого в потоке пользователей.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2b4b4519aab605978f7afba1d538d3c7007b3599
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123785"
---
# <a name="assignmentorder-resource-type"></a>тип ресурса assignmentOrder

Пространство имен: microsoft.graph

Используется для определения порядка атрибутов, собираемого в потоке пользователей. Порядок определяет отображение страницы коллекции атрибутов при записи пользователя с помощью пользовательского потока.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|порядок|Коллекция String|Список идентификаторов объектов identityUserFlowAttribute, определяющих порядок сбора атрибутов в потоке пользователей.|

## <a name="relationships"></a>Отношения

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
