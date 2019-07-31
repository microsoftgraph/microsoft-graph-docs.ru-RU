---
title: Тип ресурса office365GroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: dfc45c4973194d26c1830f8c36d3bf3b407d2e3f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009505"
---
# <a name="office365groupsactivitydetail-resource-type"></a>Тип ресурса office365GroupsActivityDetail

## <a name="properties"></a>Свойства

| Свойство                          | Тип    | Описание                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| groupId                           | String  | Идентификатор группы.          |
| Репортрефрешдате                 | Дата    | Самая поздняя дата контента.          |
| Граупдисплайнаме                  | String  | Отображаемое имя группы.           |
| isDeleted                         | Boolean | Указывает, был ли этот пользователь удален или обратимо удален. |
| ОвнерпринЦипалнаме                | String  | Имя участника владельца группы.          |
| Ластактивитидате                  | Дата    | Дата последнего действия для следующих сценариев: группового почтового ящика получено сообщение электронной почты; Пользователи, которые просматривали, редактирующие, совместно используемые или синхронизированные файлы в библиотеке документов SharePoint; страницы SharePoint, просмотренные пользователями; Разнесенные, прочитанные или понравившиеся сообщения пользователя в группах Yammer. |
| groupType                         | String  | Тип группы. Возможные значения: **Public** или **Private**. |
| Мемберкаунт                       | Int64   | Число участников группы.                  |
| Екстерналмемберкаунт               | Int64   | Количество внешних участников группы.         |
| Ексчанжерецеиведемаилкаунт        | Int64   | Количество сообщений электронной почты, принимаемых группового почтового ящика. |
| Шарепоинтактивефилекаунт         | Int64   | Количество активных файлов на сайте группы SharePoint. |
| Яммерпостедмессажекаунт          | Int64   | Количество сообщений, отправленных в группы Yammer. |
| Яммерреадмессажекаунт            | Int64   | Количество сообщений, прочитанных в группах Yammer. |
| Яммерликедмессажекаунт           | Int64   | Количество сообщений, которые понравилось в группах Yammer. |
| Ексчанжемаилбокстоталитемкаунт     | Int64   | Количество элементов в почтовом ящике группы. |
| Ексчанжемаилбокссторажеусединбитес | Int64   | Хранилище, используемое для почтового ящика группы.   |
| Шарепоинттоталфилекаунт          | Int64   | Общее количество файлов на сайте группы SharePoint. |
| Шарепоинтситесторажеусединбитес  | Int64   | Хранилище, используемое сайтом группы SharePoint. |
| Репортпериод                      | String  | Количество дней, охватываемых отчетом.    |

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
