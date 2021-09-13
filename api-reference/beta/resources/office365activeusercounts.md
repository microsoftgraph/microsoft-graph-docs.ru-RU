---
title: тип ресурса office365ActiveUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 2f11c81394dd346d46b50d2c9a19eefb56984956
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59026765"
---
# <a name="office365activeusercounts-resource-type"></a>тип ресурса office365ActiveUserCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Дата   | Последняя дата контента.          |
| office365         | Int64  | Количество активных пользователей в Microsoft 365. Этот номер включает всех активных пользователей в Exchange, OneDrive, SharePoint, Skype для бизнеса, Yammer и Microsoft Teams. Определение активного пользователя для каждого продукта можно найти в соответствующем описании свойства. |
| Exchange          | Int64  | Количество активных пользователей в Exchange. Любой пользователь, который может читать и отправлять электронную почту, считается активным пользователем. |
| oneDrive          | Int64  | Количество активных пользователей в OneDrive. Любой пользователь, который просматривал или редактировал файлы, общие файлы внутренне или внешне, или синхронизировал файлы, считается активным пользователем. |
| sharePoint        | Int64  | Количество активных пользователей в SharePoint. Любой пользователь, который просматривал или редактировал файлы, общие или внешние файлы, синхронизированные файлы или просматривал SharePoint, считается активным пользователем. |
| SkypeForBusiness  | Int64  | Количество активных пользователей в Skype для бизнеса. Любой пользователь, который организовывал или участвовал в конференциях или присоединился к одноранговых сеансах, считается активным пользователем. |
| yammer            | Int64  | Количество активных пользователей в Yammer. Любой пользователь, который может отправлять, читать или отправлять сообщения, считается активным пользователем. |
| teams             | Int64  | Количество активных пользователей в Microsoft Teams. Любой пользователь, который отправлял сообщения в каналах группы, отправлял сообщения в закрытых сеансах чата или участвовал в собраниях или звонках, считается активным пользователем. |
| reportDate        | Дата   | Дата активных действий ряда пользователей. |
| reportPeriod      | String | Количество дней, которые охватывает отчет.    |

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


