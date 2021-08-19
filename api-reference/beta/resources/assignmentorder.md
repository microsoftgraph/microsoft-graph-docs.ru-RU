---
title: тип ресурса assignmentOrder
description: Используется для определения порядка атрибутов, собираемого в потоке пользователей.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 61114b2a4fa39485843a8e1b722c518def0301ae380334f09ca79e088941040d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54245326"
---
# <a name="assignmentorder-resource-type"></a>тип ресурса assignmentOrder

Пространство имен: microsoft.graph

Используется для определения порядка атрибутов, собираемого в потоке пользователей. THis определяет отображение страницы коллекции атрибутов при записи пользователя в потоке пользователей.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|порядок|Коллекция String|Список идентификаторов identityUserFlowAttribute, предоставленных для определения порядка сбора атрибутов в потоке пользователей.|

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
