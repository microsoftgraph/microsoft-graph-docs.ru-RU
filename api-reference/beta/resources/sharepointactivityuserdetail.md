---
title: Тип ресурса Шарепоинтактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 20b99e3c6431d945200db868cc02302600e0e76c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807117"
---
# <a name="sharepointactivityuserdetail-resource-type"></a>Тип ресурса Шарепоинтактивитюсердетаил

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
| виситедпажекаунт          | Int64             |
| ассигнедпродуктс          | Коллекция String |
| репортпериод              | String            |

## <a name="json-representation"></a>Представление в формате JSON

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
