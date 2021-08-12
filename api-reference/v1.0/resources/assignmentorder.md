---
title: тип ресурса assignmentOrder
description: Определяет порядок атрибутов, собираемого в потоке пользователей.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6a68d1442135f62d7debbbed972d2187faab92188185ff5f1c6d75908ec289bd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126699"
---
# <a name="assignmentorder-resource-type"></a>тип ресурса assignmentOrder

Пространство имен: microsoft.graph

Используется для определения порядка атрибутов, собираемого в потоке пользователей. Порядок определяет отображение страницы коллекции атрибутов при записи пользователя с помощью пользовательского потока.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|порядок|Коллекция String|Список идентификаторов объектов identityUserFlowAttribute, определяющих порядок сбора атрибутов в потоке пользователей.|

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
