---
title: insightIdentity
description: Сложный тип, содержащий свойства общих элементов.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 393a6c1f7fbd1a7fffac667afcf054cdc6b54d55576ffb220df6437166827622
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229262"
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
| displayName       | String          | Отображает имя пользователя, который поделился элементом. |
| id              | String        | ID пользователя, который поделился элементом.     |
| address             | String      | Адрес электронной почты пользователя, который поделился элементом.  |

