---
title: Тип ресурса Онедривеактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 4021d1bdfb9322dbef75264ab88bb8b3a71c20e7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812150"
---
# <a name="onedriveactivityuserdetail-resource-type"></a>Тип ресурса Онедривеактивитюсердетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                  | Тип              |
| :------------------------ | :---------------- |
| репортрефрешдате         | Дата              |
| userPrincipalName         | String            |
| isDeleted                 | Логический           |
| делетеддате               | Дата              |
| ластактивитидате          | Дата              |
| виеведоредитедфилекаунт   | Int64             |
| синцедфилекаунт           | Int64             |
| шарединтерналлифилекаунт | Int64             |
| шаредекстерналлифилекаунт | Int64             |
| ассигнедпродуктс          | Коллекция String |
| репортпериод              | String            |

## <a name="json-representation"></a>Представление в формате JSON

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
