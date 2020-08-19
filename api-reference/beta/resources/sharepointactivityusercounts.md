---
title: Тип ресурса Шарепоинтактивитюсеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 70e56c30355620e1cc69f258d777e5040c9387e7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807124"
---
# <a name="sharepointactivityusercounts-resource-type"></a>Тип ресурса Шарепоинтактивитюсеркаунтс

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| репортрефрешдате | Дата   |
| виситедпаже       | Int64  |
| виеведоредитед    | Int64  |
| синхронизирован            | Int64  |
| шарединтерналли  | Int64  |
| шаредекстерналли  | Int64  |
| reportDate        | Дата   |
| репортпериод      | String |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date",
  "visitedPage": 1024,
  "viewedOrEdited": 1024,
  "synced": 1024,
  "sharedInternally": 1024,
  "sharedExternally": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
