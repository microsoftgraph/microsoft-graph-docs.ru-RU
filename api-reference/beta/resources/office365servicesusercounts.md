---
title: Тип ресурса office365ServicesUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 276153f9613f464cdf11f6dfdad307bb341f646d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982154"
---
# <a name="office365servicesusercounts-resource-type"></a>Тип ресурса office365ServicesUserCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                 | Тип   | Описание                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Дата   | Последняя дата содержимого.          |
| exchangeActive           | Int64  | Количество активных пользователей в Exchange. Любой пользователь, который может читать и отправлять электронную почту, считается активным пользователем. |
| exchangeInactive         | Int64  | Количество неактивных пользователей в Exchange. |
| oneDriveActive           | Int64  | Количество активных пользователей в OneDrive. Любой пользователь, просматривавший или редактировал файлы, общие файлы внутри или извне или синхронизированные файлы, считается активным пользователем. |
| oneDriveInactive         | Int64  | Количество неактивных пользователей в OneDrive. |
| sharePointActive         | Int64  | Количество активных пользователей в SharePoint. Любой пользователь, который просматривал или редактировал файлы, общие файлы внутри или извне, синхронизированные файлы или просматривал страницы SharePoint, считается активным пользователем. |
| sharePointInactive       | Int64  | Количество неактивных пользователей в SharePoint. |
| skypeForBusinessActive   | Int64  | Количество активных пользователей в Skype для бизнеса. Любой пользователь, который организовывал или принимал участие в конференциях или присоединялся к одноранговом сеансу, считается активным пользователем. |
| skypeForBusinessInactive | Int64  | Количество неактивных пользователей в Skype для бизнеса. |
| yammerActive             | Int64  | Количество активных пользователей в Yammer. Любой пользователь, который может размещать, читать или читать сообщения, считается активным пользователем. |
| yammerInactive           | Int64  | Количество неактивных пользователей в Yammer.  |
| teamsActive              | Int64  | Количество активных пользователей в Microsoft Teams. Любой пользователь, который опубликовал сообщения в каналах группы, отправил сообщения в сеансах приватного чата или участвовал в собраниях или звонках, считается активным пользователем. |
| teamsInactive            | Int64  | Количество неактивных пользователей в Microsoft Teams.     |
| office365Active          | Int64  | Количество активных пользователей в Microsoft 365.   |
| office365Inactive        | Int64  | Количество неактивных пользователей в Microsoft 365.     |
| reportPeriod             | String | Количество дней в отчете.    |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeActive": 1024, 
  "exchangeInactive": 1024, 
  "oneDriveActive": 1024, 
  "oneDriveInactive": 1024, 
  "sharePointActive": 1024, 
  "sharePointInactive": 1024, 
  "skypeForBusinessActive": 1024, 
  "skypeForBusinessInactive": 1024, 
  "yammerActive": 1024, 
  "yammerInactive": 1024, 
  "teamsActive": 1024, 
  "teamsInactive": 1024, 
  "office365Active": 1024,
  "office365Inactive": 1024,
  "reportPeriod": "String"
}
```


