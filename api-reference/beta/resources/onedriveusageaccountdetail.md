---
title: Тип ресурса Онедривеусажеаккаунтдетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c13e03d1170b0ebbc53394541c4564c60c67e78
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563548"
---
# <a name="onedriveusageaccountdetail-resource-type"></a>Тип ресурса Онедривеусажеаккаунтдетаил

## <a name="properties"></a>Свойства

| Свойство                | Тип    |
| :---------------------- | :------ |
| Репортрефрешдате       | Дата    |
| siteUrl                 | String  |
| Овнердисплайнаме        | String  |
| isDeleted               | Boolean |
| Ластактивитидате        | Дата    |
| Филекаунт               | Int64   |
| Активефилекаунт         | Int64   |
| Сторажеусединбитес      | Int64   |
| Сторажеаллокатединбитес | Int64   |
| Репортпериод            | String  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteUrl": "String", 
  "ownerDisplayName": "String", 
  "isDeleted": true, 
  "lastActivityDate": "Date", 
  "fileCount": 1024, 
  "activeFileCount": 1024, 
  "storageUsedInBytes": 1024, 
  "storageAllocatedInBytes": 1024, 
  "reportPeriod": "String"
}
```
