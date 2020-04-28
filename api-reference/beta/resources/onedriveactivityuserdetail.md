---
title: Тип ресурса Онедривеактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 22702a392a76a21951c24667da0e8a1e61c8b36c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522395"
---
# <a name="onedriveactivityuserdetail-resource-type"></a>Тип ресурса Онедривеактивитюсердетаил

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
| ассигнедпродуктс          | Коллекция объектов string |
| репортпериод              | String            |

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
