---
title: insightIdentity
description: Сложный тип, содержащий свойства общих элементов.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3a23344a18979c7d1aa69b8e841007812797b238
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531299"
---
# <a name="insightidentity"></a>insightIdentity

Пространство имен: microsoft.graph

Сложный тип, содержащий свойства элементов [шарединсигхт](insights-shared.md) . 

## <a name="json-representation"></a>Представление JSON
Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.insightIdentity"
}-->
```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a>Свойства

| Свойство              | Тип          | Описание  |
| -------------         |-----------    | -------------|
| displayName       | Строка          | Отображаемое имя пользователя, который предоставил общий доступ к элементу. |
| id              | String        | Идентификатор пользователя, который предоставил общий доступ к элементу.     |
| address             | String      | Адрес электронной почты пользователя, который предоставил общий доступ к элементу.  |
