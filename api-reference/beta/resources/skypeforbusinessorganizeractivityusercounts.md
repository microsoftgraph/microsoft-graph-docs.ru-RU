---
title: Тип ресурса Скипефорбусинессорганизерактивитюсеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b6fcb2114e78bd9aabb170795b49d80bb58e6844
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964874"
---
# <a name="skypeforbusinessorganizeractivityusercounts-resource-type"></a>Тип ресурса Скипефорбусинессорганизерактивитюсеркаунтс

## <a name="properties"></a>Свойства

| Свойство           | Тип   |
| :----------------- | :----- |
| im                 | Int64  |
| Audiovideohttp         | Int64  |
| Аппшаринг         | Int64  |
| web                | Int64  |
| dialInOut3rdParty  | Int64  |
| Диалинаутмикрософт | Int64  |
| Репортрефрешдате  | Дата   |
| reportDate         | Дата   |
| Репортпериод       | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityUserCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 1024, 
  "appSharing": 1024, 
  "web": 1024, 
  "dialInOut3rdParty": 1024, 
  "dialInOutMicrosoft": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
