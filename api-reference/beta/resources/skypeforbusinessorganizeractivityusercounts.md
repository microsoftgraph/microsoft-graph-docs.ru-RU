---
title: Тип ресурса Скипефорбусинессорганизерактивитюсеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 39ab5844adb9525b4e0f100892927d200609040c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534866"
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

## <a name="json-representation"></a>Представление в формате JSON

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
