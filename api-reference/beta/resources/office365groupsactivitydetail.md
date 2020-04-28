---
title: Тип ресурса office365GroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: d517763fdfcbf046c36fc944d229b9a15b0cb8fd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522451"
---
# <a name="office365groupsactivitydetail-resource-type"></a>Тип ресурса office365GroupsActivityDetail

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                          | Тип    | Описание                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| groupId                           | String  | Идентификатор группы.          |
| репортрефрешдате                 | Дата    | Самая поздняя дата контента.          |
| граупдисплайнаме                  | String  | Отображаемое имя группы.           |
| isDeleted                         | Boolean | Указывает, был ли этот пользователь удален или обратимо удален. |
| овнерпринЦипалнаме                | String  | Имя участника владельца группы.          |
| ластактивитидате                  | Дата    | Дата последнего действия для следующих сценариев: группового почтового ящика получено сообщение электронной почты; Пользователи, которые просматривали, редактирующие, совместно используемые или синхронизированные файлы в библиотеке документов SharePoint; страницы SharePoint, просмотренные пользователями; Разнесенные, прочитанные или понравившиеся сообщения пользователя в группах Yammer. |
| groupType                         | String  | Тип группы. Возможные значения: **Public** или **Private**. |
| мемберкаунт                       | Int64   | Число участников группы.                  |
| екстерналмемберкаунт               | Int64   | Количество внешних участников группы.         |
| ексчанжерецеиведемаилкаунт        | Int64   | Количество сообщений электронной почты, принимаемых группового почтового ящика. |
| шарепоинтактивефилекаунт         | Int64   | Количество активных файлов на сайте группы SharePoint. |
| яммерпостедмессажекаунт          | Int64   | Количество сообщений, отправленных в группы Yammer. |
| яммерреадмессажекаунт            | Int64   | Количество сообщений, прочитанных в группах Yammer. |
| яммерликедмессажекаунт           | Int64   | Количество сообщений, которые понравилось в группах Yammer. |
| ексчанжемаилбокстоталитемкаунт     | Int64   | Количество элементов в почтовом ящике группы. |
| ексчанжемаилбокссторажеусединбитес | Int64   | Хранилище, используемое для почтового ящика группы.   |
| шарепоинттоталфилекаунт          | Int64   | Общее количество файлов на сайте группы SharePoint. |
| шарепоинтситесторажеусединбитес  | Int64   | Хранилище, используемое сайтом группы SharePoint. |
| репортпериод                      | String  | Количество дней, охватываемых отчетом.    |

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
