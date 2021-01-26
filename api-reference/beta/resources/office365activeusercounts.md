---
title: Тип ресурса office365ActiveUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 67c9b898da9a106685739ebbf78ccef6425c6617
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980740"
---
# <a name="office365activeusercounts-resource-type"></a>Тип ресурса office365ActiveUserCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Дата   | Последняя дата содержимого.          |
| office365         | Int64  | Количество активных пользователей в Microsoft 365. Это число включает всех активных пользователей в Exchange, OneDrive, SharePoint, Skype для бизнеса, Yammer и Microsoft Teams. Определение активного пользователя для каждого продукта можно найти в соответствующем описании свойства. |
| exchange          | Int64  | Количество активных пользователей в Exchange. Любой пользователь, который может читать и отправлять электронную почту, считается активным пользователем. |
| oneDrive          | Int64  | Количество активных пользователей в OneDrive. Любой пользователь, который просматривал или редактировал файлы, общие файлы внутри или извне или синхронизированные файлы, считается активным пользователем. |
| sharePoint        | Int64  | Количество активных пользователей в SharePoint. Любой пользователь, который просматривал или редактировал файлы, общие файлы внутри или извне, синхронизированные файлы или просматривал страницы SharePoint, считается активным пользователем. |
| skypeForBusiness  | Int64  | Количество активных пользователей в Skype для бизнеса. Любой пользователь, который организовывал или принимал участие в конференциях или присоединялся к одноранговом сеансу, считается активным пользователем. |
| yammer            | Int64  | Количество активных пользователей в Yammer. Любой пользователь, который может размещать, читать или читать сообщения, считается активным пользователем. |
| teams             | Int64  | Количество активных пользователей в Microsoft Teams. Любой пользователь, который опубликовал сообщения в каналах группы, отправил сообщения в сеансах приватного чата или участвовал в собраниях или звонках, считается активным пользователем. |
| reportDate        | Дата   | Дата, когда было активно несколько пользователей. |
| reportPeriod      | String | Количество дней в отчете.    |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "office365": 1024, 
  "exchange": 1024, 
  "oneDrive": 1024, 
  "sharePoint": 1024, 
  "skypeForBusiness": 1024, 
  "yammer": 1024, 
  "teams": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


