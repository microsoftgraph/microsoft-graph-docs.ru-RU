---
title: тип ресурса office365GroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 0d32d6c44c520f3dd7fe88494da4bfecc0d1ad14
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61863531"
---
# <a name="office365groupsactivitydetail-resource-type"></a>тип ресурса office365GroupsActivityDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>Свойства

| Свойство                          | Тип    | Описание                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| groupId                           | String  | ID группы.          |
| reportRefreshDate                 | Дата    | Последняя дата контента.          |
| groupDisplayName                  | String  | Отображает имя группы.           |
| isDeleted                         | Логический | Был ли этот пользователь удален или удален. |
| ownerPrincipalName                | String  | Имя основного владельца группы.          |
| lastActivityDate                  | Дата    | Последняя дата действий для следующих сценариев: почтовый ящик группы получил электронную почту; просмотр, редактирование, общий доступ или синхронизация файлов в библиотеке SharePoint документов; просмотр SharePoint страниц; публикация, чтение или просмотр сообщений в Yammer группах. |
| groupType                         | String  | Тип группы. Возможные значения: **общедоступные или** **частные.** |
| memberCount                       | Int64   | Количество членов группы.                  |
| externalMemberCount               | Int64   | Количество внешних членов группы.         |
| exchangeReceivedEmailCount        | Int64   | Количество сообщений электронной почты, полученных почтовым ящиком группы. |
| sharePointActiveFileCount         | Int64   | Количество активных файлов на сайте SharePoint Group. |
| yammerPostedMessageCount          | Int64   | Количество сообщений, которые были размещены в Yammer группах. |
| yammerReadMessageCount            | Int64   | Количество сообщений, читаемых в Yammer группах. |
| yammerLikedMessageCount           | Int64   | Количество сообщений, которые нравятся в Yammer группах. |
| exchangeMailboxTotalItemCount     | Int64   | Количество элементов в почтовом ящике группы. |
| exchangeMailboxStorageUsedInBytes | Int64   | Хранилище, используемого для группового почтового ящика.   |
| sharePointTotalFileCount          | Int64   | Общее количество файлов на сайте SharePoint Group. |
| sharePointSiteStorageUsedInBytes  | Int64   | Хранилище, используемого SharePoint Group. |
| reportPeriod                      | String  | Количество дней, которые охватывает отчет.    |

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


