---
title: insightIdentity
description: Сложный тип, содержащий свойства общих элементов.
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 701840cea5f1bc5e878e5d47c21caf97aed320de
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129868"
---
# <a name="insightidentity"></a>insightIdentity

Пространство имен: microsoft.graph

Сложный тип, содержащий свойства [элементов sharedInsight.](insights-shared.md) 

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
| displayName       | Строка          | Отображает имя пользователя, который поделился элементом. |
| id              | String        | ID пользователя, который поделился элементом.     |
| address             | String      | Адрес электронной почты пользователя, который поделился элементом.  |

