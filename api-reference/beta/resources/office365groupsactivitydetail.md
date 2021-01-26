---
title: Тип ресурса office365GroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: fe2df5614525f27b294bed93be7f3f9cd8170b30
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981510"
---
# <a name="office365groupsactivitydetail-resource-type"></a>Тип ресурса office365GroupsActivityDetail

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                          | Тип    | Описание                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| groupId                           | String  | ИД группы.          |
| reportRefreshDate                 | Дата    | Последняя дата содержимого.          |
| groupDisplayName                  | String  | Отображаемого имени группы.           |
| isDeleted                         | Boolean | Был ли этот пользователь удален или удален с помягким образом. |
| ownerPrincipalName                | String  | Имя владельца группы.          |
| lastActivityDate                  | Дата    | Дата последнего действия для следующих сценариев: почтовый ящик группы получил сообщение электронной почты; просматриваются, редактируются, совместно или синхронизируются файлы в библиотеке документов SharePoint; просматривались пользователем страницы SharePoint; пользователи опубликовали, прочитали или понравились сообщения в группах Yammer. |
| groupType                         | String  | Тип группы. Возможные значения: **Public или** **Private**. |
| memberCount                       | Int64   | Количество членов группы.                  |
| externalMemberCount               | Int64   | Количество внешних членов группы.         |
| exchangeReceivedEmailCount        | Int64   | Количество сообщений электронной почты, полученных почтовым ящиком группы. |
| sharePointActiveFileCount         | Int64   | Количество активных файлов на сайте группы SharePoint. |
| yammerPostedMessageCount          | Int64   | Количество сообщений, которые были опубликованы в группах Yammer. |
| yammerReadMessageCount            | Int64   | Количество сообщений, прочитано в группах Yammer. |
| yammerАedMessageCount           | Int64   | Количество сообщений, которые нравится в группах Yammer. |
| exchangeMailboxTotalItemCount     | Int64   | Количество элементов в почтовом ящике группы. |
| exchangeMailboxStorageUsedInBytes | Int64   | Хранилище, используемого почтовым ящиком группы.   |
| sharePointTotalFileCount          | Int64   | Общее количество файлов на сайте группы SharePoint. |
| sharePointSiteStorageUsedInBytes  | Int64   | Хранилище, используемого сайтом группы SharePoint. |
| reportPeriod                      | String  | Количество дней в отчете.    |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
  "groupId": "0003cf63-7ff3-4471-b24b-50ffbfb8b5d2",
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "memberCount": 1024, 
  "externalMemberCount": 1024, 
  "exchangeReceivedEmailCount": 1024, 
  "sharePointActiveFileCount": 1024, 
  "yammerPostedMessageCount": 1024, 
  "yammerReadMessageCount": 1024, 
  "yammerLikedMessageCount": 1024, 
  "exchangeMailboxTotalItemCount": 1024, 
  "exchangeMailboxStorageUsedInBytes": 1024, 
  "sharePointTotalFileCount": 1024, 
  "sharePointSiteStorageUsedInBytes": 1024, 
  "reportPeriod": "String"
}
```


