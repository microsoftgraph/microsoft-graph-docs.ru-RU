---
title: Тип ресурса Скипефорбусинессорганизерактивитиминутекаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 6b3b38c61ebb7b294de9ea5fc2641a7527bf04f7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461187"
---
# <a name="skypeforbusinessorganizeractivityminutecounts-resource-type"></a>Тип ресурса Скипефорбусинессорганизерактивитиминутекаунтс

## <a name="properties"></a>Свойства

| Свойство           | Тип   |
| :----------------- | :----- |
| Audiovideohttp         | Int64  |
| dialInOut3rdParty  | Int64  |
| Диалинаутмикрософт | Int64  |
| Репортрефрешдате  | Дата   |
| reportDate         | Дата   |
| Репортпериод       | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts"
} -->

```json
{
  "audioVideo": 1024, 
  "dialInMicrosoft": 1024, 
  "dialOutMicrosoft": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
