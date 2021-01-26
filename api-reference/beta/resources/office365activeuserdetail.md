---
title: Тип ресурса office365ActiveUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 057490d5e19a8e56a2e83047277292fbd0af4a16
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980691"
---
# <a name="office365activeuserdetail-resource-type"></a>Тип ресурса office365ActiveUserDetail

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                          | Тип              | Описание                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| reportRefreshDate                 | Дата              | Последняя дата содержимого.          |
| userPrincipalName                 | String            | Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. |
| displayName                       | String            | Имя пользователя, отображаемое в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. |
| isDeleted                         | Boolean           | Был ли этот пользователь удален или удален с помягким образом. |
| deletedDate                       | Дата              | Дата операции удаления. Значение по умолчанию — null, если пользователь не был удален. |
| hasExchangeLicense                | Boolean           | Назначена ли пользователю лицензия Exchange. |
| hasOneDriveLicense                | Boolean           | Назначена ли пользователю лицензия на OneDrive. |
| hasSharePointLicense              | Boolean           | Назначена ли пользователю лицензия SharePoint. |
| hasSkypeForBusinessLicense        | Boolean           | Назначена ли пользователю лицензия Skype для бизнеса. |
| hasYammerLicense                  | Boolean           | Назначена ли пользователю лицензия на Yammer. |
| hasTeamsLicense                   | Boolean           | Назначена ли пользователю лицензия Teams. |
| exchangeLastActivityDate          | Дата              | Дата последнего чтения или отправки пользователем сообщения электронной почты. |
| oneDriveLastActivityDate          | Дата              | Дата последнего просмотра или изменения пользователем файлов, общих файлов внутри или извне или синхронизированных файлов. |
| sharePointLastActivityDate        | Дата              | Дата последнего просмотра или изменения пользователем файлов, общих файлов внутри или извне, синхронизированных файлов или просмотров страниц SharePoint. |
| skypeForBusinessLastActivityDate  | Дата              | Дата последней организации или участия пользователя в конференциях или в одноранговых сеансах. |
| yammerLastActivityDate            | Дата              | Дата последней публикации, чтения или понравившейся публикации сообщения пользователем. |
| teamsLastActivityDate             | Дата              | Дата последней публикации сообщений в каналах группы, сообщений в сеансах закрытого чата или участия в собраниях или звонках. |
| exchangeLicenseAssignDate         | Дата              | Дата последней даты, когда пользователю была назначена лицензия Exchange. |
| oneDriveLicenseAssignDate         | Дата              | Дата последней даты, когда пользователю была назначена лицензия на OneDrive. |
| sharePointLicenseAssignDate       | Дата              | Дата последнего назначения пользователю лицензии SharePoint. |
| skypeForBusinessLicenseAssignDate | Дата              | Дата последней даты, когда пользователю была назначена лицензия Skype для бизнеса. |
| yammerLicenseAssignDate           | Дата              | Дата последней даты, когда пользователю была назначена лицензия на Yammer. |
| teamsLicenseAssignDate            | Дата              | Дата последней даты, когда пользователю была назначена лицензия Teams. |
| assignedProducts                  | Коллекция String | Все продукты, которые назначены пользователю.  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "hasExchangeLicense": true, 
  "hasOneDriveLicense": true, 
  "hasSharePointLicense": true, 
  "hasSkypeForBusinessLicense": true, 
  "hasYammerLicense": true, 
  "hasTeamsLicense": true, 
  "exchangeLastActivityDate": "Date", 
  "oneDriveLastActivityDate": "Date", 
  "sharePointLastActivityDate": "Date", 
  "skypeForBusinessLastActivityDate": "Date", 
  "yammerLastActivityDate": "Date", 
  "teamsLastActivityDate": "Date", 
  "exchangeLicenseAssignDate": "Date", 
  "oneDriveLicenseAssignDate": "Date", 
  "sharePointLicenseAssignDate": "Date", 
  "skypeForBusinessLicenseAssignDate": "Date", 
  "yammerLicenseAssignDate": "Date", 
  "teamsLicenseAssignDate": "Date", 
  "assignedProducts": ["String"]
}
```


