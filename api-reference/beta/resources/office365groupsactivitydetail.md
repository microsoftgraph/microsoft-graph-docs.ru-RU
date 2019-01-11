---
title: Тип ресурса office365GroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 94dc10064c0005770294c8f783c77d41ce0c479b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894273"
---
# <a name="office365groupsactivitydetail-resource-type"></a>Тип ресурса office365GroupsActivityDetail

## <a name="properties"></a>Свойства

| Свойство                          | Тип    | Описание                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| reportRefreshDate                 | Date    | Последняя дата контента.          |
| groupDisplayName                  | Строка  | Отображаемое имя группы.           |
| isDeleted                         | Логический | Был ли этот пользователь удаленного или программных удалены. |
| ownerPrincipalName                | Строка  | Имя участника группы владельца.          |
| lastActivityDate                  | Date    | Дата последнего действия для следующих сценариев: групповой полученных почтового ящика электронной почты; пользователю просматривать, редактировать, общих или синхронизирован файлы в библиотеке документов SharePoint. пользователь просматривает страницы SharePoint; пользователь учтена, чтение или оцененных сообщений в группах Yammer. |
| groupType                         | Строка  | Тип группы. Возможные значения: **Public** или **Private**. |
| memberCount                       | Int64   | Счетчик членов группы.                  |
| externalMemberCount               | Int64   | Счетчик внешнего участника группы.         |
| exchangeReceivedEmailCount        | Int64   | Число электронной почты, полученных почтового ящика группы. |
| sharePointActiveFileCount         | Int64   | Число активных файлов на сайте группы SharePoint. |
| yammerPostedMessageCount          | Int64   | Число сообщений, помещенных в группы Yammer. |
| yammerReadMessageCount            | Int64   | Количество сообщений, ознакомьтесь с разделом в группы Yammer. |
| yammerLikedMessageCount           | Int64   | Количество сообщений, оцененных в группах Yammer. |
| exchangeMailboxTotalItemCount     | Int64   | Количество элементов в почтовом ящике группы. |
| exchangeMailboxStorageUsedInBytes | Int64   | Хранения, используемый для почтового ящика группы.   |
| sharePointTotalFileCount          | Int64   | Общее число файлов на сайте группы SharePoint. |
| sharePointSiteStorageUsedInBytes  | Int64   | Хранилище, используемое сайта группы SharePoint. |
| reportPeriod                      | Строка  | Количество дней, на которое отчета.    |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
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
