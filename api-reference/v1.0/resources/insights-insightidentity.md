---
title: insightIdentity
description: Сложный тип, содержащий свойства общих элементов.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 1dc952ba931e1a0cb4302dac881f2d5ec015c591
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844436"
---
# <a name="insightidentity"></a>insightIdentity

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
