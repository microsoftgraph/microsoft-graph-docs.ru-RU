---
title: тип ресурса office365ServicesUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 6470804a26a35b1aaf8411d5c0d5fddd2a3e0bbf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59095327"
---
# <a name="office365servicesusercounts-resource-type"></a>тип ресурса office365ServicesUserCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                 | Тип   | Описание                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Дата   | Последняя дата контента.          |
| ExchangeActive           | Int64  | Количество активных пользователей на Exchange. Любой пользователь, который может читать и отправлять электронную почту, считается активным пользователем. |
| ExchangeInactive         | Int64  | Количество неактивных пользователей на Exchange. |
| oneDriveActive           | Int64  | Количество активных пользователей на OneDrive. Любой пользователь, который просматривал или редактировал файлы, общие файлы внутренне или внешне, или синхронизировал файлы, считается активным пользователем. |
| oneDriveInactive         | Int64  | Количество неактивных пользователей в OneDrive. |
| sharePointActive         | Int64  | Количество активных пользователей на SharePoint. Любой пользователь, который просматривал или редактировал файлы, общие или внешние файлы, синхронизированные файлы или просматривал SharePoint, считается активным пользователем. |
| sharePointInactive       | Int64  | Количество неактивных пользователей в SharePoint. |
| SkypeForBusinessActive   | Int64  | Количество активных пользователей в Skype для бизнеса. Любой пользователь, который организовывал или участвовал в конференциях или присоединился к одноранговых сеансах, считается активным пользователем. |
| SkypeForBusinessInactive | Int64  | Количество неактивных пользователей в Skype для бизнеса. |
| yammerActive             | Int64  | Количество активных пользователей на Yammer. Любой пользователь, который может отправлять, читать или отправлять сообщения, считается активным пользователем. |
| yammerInactive           | Int64  | Количество неактивных пользователей на Yammer.  |
| teamsActive              | Int64  | Количество активных пользователей на Microsoft Teams. Любой пользователь, который отправлял сообщения в каналах группы, отправлял сообщения в закрытых сеансах чата или участвовал в собраниях или звонках, считается активным пользователем. |
| teamsInactive            | Int64  | Количество неактивных пользователей на Microsoft Teams.     |
| office365Active          | Int64  | Количество активных пользователей на Microsoft 365.   |
| office365Inactive        | Int64  | Количество неактивных пользователей в Microsoft 365.     |
| reportPeriod             | String | Количество дней, которые охватывает отчет.    |

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


