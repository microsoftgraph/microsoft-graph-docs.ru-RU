---
title: Тип ресурса Шарепоинтактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 7394e2fab0604286e8066b64e86f413f421472cf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997797"
---
# <a name="sharepointactivityuserdetail-resource-type"></a>Тип ресурса Шарепоинтактивитюсердетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                  | Тип              |
| :------------------------ | :---------------- |
| репортрефрешдате         | Дата              |
| userPrincipalName         | String            |
| isDeleted                 | Boolean           |
| делетеддате               | Дата              |
| ластактивитидате          | Дата              |
| виеведоредитедфилекаунт   | Int64             |
| синцедфилекаунт           | Int64             |
| шарединтерналлифилекаунт | Int64             |
| шаредекстерналлифилекаунт | Int64             |
| виситедпажекаунт          | Int64             |
| ассигнедпродуктс          | Коллекция String |
| репортпериод              | String            |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date",
  "userPrincipalName": "String",
  "isDeleted": true,
  "deletedDate": "Date",
  "lastActivityDate": "Date",
  "viewedOrEditedFileCount": 1024,
  "syncedFileCount": 1024,
  "sharedInternallyFileCount": 1024,
  "sharedExternallyFileCount": 1024,
  "visitedPageCount": 1024,
  "assignedProducts": ["String"],
  "reportPeriod": "String"
}
```


