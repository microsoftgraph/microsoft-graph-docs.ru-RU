---
title: тип ресурса assignmentOrder
description: Используется для определения порядка атрибутов, собираемого в потоке пользователей.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: afc59c24e154e8349eacff0d4059f1b102d8bc19
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033835"
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
