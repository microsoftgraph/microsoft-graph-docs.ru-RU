---
title: Тип ресурса Шарепоинтактивитюсеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9656b39572eac5b6474dd7884eb7d1d2edb17310
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583951"
---
# <a name="sharepointactivityusercounts-resource-type"></a>Тип ресурса Шарепоинтактивитюсеркаунтс

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| Репортрефрешдате | Дата   |
| Виситедпаже       | Int64  |
| Виеведоредитед    | Int64  |
| синхронизирован            | Int64  |
| Шарединтерналли  | Int64  |
| Шаредекстерналли  | Int64  |
| reportDate        | Дата   |
| Репортпериод      | String |

## <a name="json-representation"></a>Представление JSON

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
