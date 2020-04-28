---
title: insightIdentity
description: Сложный тип, содержащий свойства общих элементов.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: fee67727e610e44ab8cfcf15f973160310575136
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495874"
---
# <a name="insightidentity"></a>insightIdentity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
