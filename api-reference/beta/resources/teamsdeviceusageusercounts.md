---
title: тип ресурса teamsDeviceUsageUserCounts
description: Представляет число ежедневных пользователей по типу устройства.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9d7b813727a5ac9b2f7547e108bad8ee455d206b
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766576"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a>тип ресурса teamsDeviceUsageUserCounts

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет число ежедневных пользователей по типу устройства.

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                                                  |
| :---------------- | :----- | ------------------------------------------------------------ |
| reportRefreshDate | Дата   | Последняя дата контента.                              |
| web               | Int64  | Количество пользователей, активных в веб-клиенте Teams на устройствах. |
| WindowsPhone      | Int64  | Количество пользователей, активных в мобильном клиенте Teams для телефона Windows. |
| AndroidPhone      | Int64  | Количество пользователей, активных в мобильном клиенте Teams для Android. |
| ios               | Int64  | Количество пользователей, активных в мобильном клиенте Teams для iOS. |
| mac               | Int64  | Число пользователей, активных в клиенте Teams на компьютере macOS. |
| Windows           | Int64  | Количество пользователей, активных в клиенте teams на компьютере с Windows. |
| chromeOS          | Int64  | Количество пользователей, активных в клиенте teams на компьютере ChromeOS. |
| Linux             | Int64  | Количество пользователей, которые были активны в клиенте настольных компьютеров Teams на компьютере Linux. |
| reportDate        | Дата   | Дата выполнения пользователями действий.        |
| reportPeriod      | String | Количество дней, которые охватывает отчет.                        |

## <a name="representation"></a>представление

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "chromeOS": 1024, 
  "linux": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


