---
title: Тип ресурса sharePointActivityUserDetail
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: a5b6de8a4a9b82d9e6d34a2ae289f0c7589798ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075477"
---
# <a name="sharepointactivityuserdetail-resource-type"></a>Тип ресурса sharePointActivityUserDetail

## <a name="properties"></a>Свойства

| Свойство                  | Тип              |
| :------------------------ | :---------------- |
| reportRefreshDate         | Date              |
| userPrincipalName         | String            |
| isDeleted                 | Логический           |
| deletedDate               | Date              |
| lastActivityDate          | Date              |
| viewedOrEditedFileCount   | Int64             |
| syncedFileCount           | Int64             |
| sharedInternallyFileCount | Int64             |
| sharedExternallyFileCount | Int64             |
| visitedPageCount          | Int64             |
| assignedProducts          | Коллекция String |
| reportPeriod              | String            |

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
