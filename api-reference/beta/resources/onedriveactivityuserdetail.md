---
title: Тип ресурса Онедривеактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 29c9c8b723d4f87fa9858e26906878c973b37b09
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582250"
---
# <a name="onedriveactivityuserdetail-resource-type"></a>Тип ресурса Онедривеактивитюсердетаил

## <a name="properties"></a>Свойства

| Свойство                  | Тип              |
| :------------------------ | :---------------- |
| Репортрефрешдате         | Дата              |
| userPrincipalName         | String            |
| isDeleted                 | Boolean           |
| Делетеддате               | Дата              |
| Ластактивитидате          | Дата              |
| Виеведоредитедфилекаунт   | Int64             |
| Синцедфилекаунт           | Int64             |
| Шарединтерналлифилекаунт | Int64             |
| Шаредекстерналлифилекаунт | Int64             |
| Ассигнедпродуктс          | Коллекция String |
| Репортпериод              | String            |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
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
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
