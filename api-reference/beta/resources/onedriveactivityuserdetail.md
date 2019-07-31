---
title: Тип ресурса Онедривеактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: c61db94678ed50e6cc93f123a506ce262616a1ab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966484"
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
| Ассигнедпродуктс          | Коллекция строк |
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
