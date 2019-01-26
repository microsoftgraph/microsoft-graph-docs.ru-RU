---
title: Тип ресурса office365ServicesUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 36fd043be3cef36951f7651d625f4a93d3b5f8cc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573895"
---
# <a name="office365servicesusercounts-resource-type"></a>Тип ресурса office365ServicesUserCounts

## <a name="properties"></a>Свойства

| Свойство                 | Тип   | Описание                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Date   | Последняя дата контента.          |
| exchangeActive           | Int64  | Число активных пользователей на сервере Exchange. Любой пользователь, который можно читать и отправлять электронную почту считается активного пользователя. |
| exchangeInactive         | Int64  | Количество неактивных пользователей на сервере Exchange. |
| oneDriveActive           | Int64  | Количество активных пользователей на OneDrive. Любой пользователь, просматривать или изменять файлы, общих файлов во внутреннем или внешнем ресурсе или синхронизирован файлы считается активного пользователя. |
| oneDriveInactive         | Int64  | Количество неактивных пользователей на OneDrive. |
| sharePointActive         | Int64  | Число активных пользователей в SharePoint. Любой пользователь, просматривать или изменять файлы, общих файлов во внутренней сети или извне, синхронизированные файлы или просматривать страницы SharePoint считается активного пользователя. |
| sharePointInactive       | Int64  | Количество неактивных пользователей на сайте SharePoint. |
| skypeForBusinessActive   | Int64  | Число активных пользователей в Скайп для бизнеса. Любой пользователь, который организовал принявших участие в конференциях или в состав peer-to-peer sessions считается активного пользователя. |
| skypeForBusinessInactive | Int64  | Количество неактивных пользователей на Скайп для бизнеса. |
| yammerActive             | Int64  | Число активных пользователей в Yammer. Любой пользователь, который можно публиковать, чтение или как сообщения считается активного пользователя. |
| yammerInactive           | Int64  | Количество неактивных пользователей в Yammer.  |
| teamsActive              | Int64  | Число активных пользователей в группы Microsoft. Любой пользователь, который сообщений, помещенных в каналы группы, отправленных сообщений в сеансах частной беседы или являлся участником собрания или вызовы считается активного пользователя. |
| teamsInactive            | Int64  | Количество неактивных пользователей на группами Майкрософт.     |
| office365Active          | Int64  | Число активных пользователей в Office 365.   |
| office365Inactive        | Int64  | Количество неактивных пользователей на Office 365.     |
| reportPeriod             | Строка | Количество дней, на которое отчета.    |

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
