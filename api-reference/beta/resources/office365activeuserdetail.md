---
title: тип ресурса office365ActiveUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 0fecf7811bd7f72f80f8b95fa89cfb75387f8ec88374066d41ffea9e0e6ad338
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54214826"
---
# <a name="office365activeuserdetail-resource-type"></a>тип ресурса office365ActiveUserDetail

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                          | Тип              | Описание                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| reportRefreshDate                 | Дата              | Последняя дата контента.          |
| userPrincipalName                 | String            | Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. |
| displayName                       | String            | Имя пользователя, отображаемое в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. |
| isDeleted                         | Логический           | Был ли этот пользователь удален или удален. |
| deletedDate                       | Дата              | Дата, когда произошла операция удаления. Значение по умолчанию — "null", если пользователь не удален. |
| hasExchangeLicense                | Логический           | Назначено ли пользователю Exchange лицензии. |
| hasOneDriveLicense                | Логический           | Назначена ли пользователю OneDrive лицензия. |
| hasSharePointLicense              | Логический           | Назначена ли пользователю SharePoint лицензия. |
| hasSkypeForBusinessLicense        | Логический           | Назначена ли пользователю лицензия Skype для бизнеса. |
| hasYammerLicense                  | Логический           | Назначена ли пользователю Yammer лицензия. |
| hasTeamsLicense                   | Логический           | Назначена ли пользователю Teams лицензия. |
| exchangeLastActivityDate          | Дата              | Дата последнего чтения или отправки электронной почты пользователем. |
| oneDriveLastActivityDate          | Дата              | Дата последнего просмотра или редактирования файлов пользователя, внутренних или внешних общих файлов или синхронизированных файлов. |
| sharePointLastActivityDate        | Дата              | Дата последнего просмотра или редактирования файлов пользователя, внутренних или внешних, синхронизированных файлов или SharePoint страниц. |
| SkypeForBusinessLastActivityDate  | Дата              | Дата, когда пользователь последний раз организовывал или участвовал в конференциях или присоединялся к одноранговых сеансам. |
| yammerLastActivityDate            | Дата              | Дата последнего опубликования, чтения или понравившейся сообщения пользователем. |
| teamsLastActivityDate             | Дата              | Дата последней публикации сообщений пользователем в каналах группы, отправление сообщений в закрытых сеансах чата или участие в собраниях или звонках. |
| exchangeLicenseAssignDate         | Дата              | Последняя дата, когда пользователю была назначена Exchange лицензия. |
| oneDriveLicenseAssignDate         | Дата              | Последняя дата, когда пользователю была назначена OneDrive лицензия. |
| sharePointLicenseAssignDate       | Дата              | Последняя дата, когда пользователю была назначена SharePoint лицензия. |
| SkypeForBusinessLicenseAssignDate | Дата              | Последняя дата, когда пользователю была назначена Skype для бизнеса. |
| yammerLicenseAssignDate           | Дата              | Последняя дата, когда пользователю была назначена Yammer лицензия. |
| teamsLicenseAssignDate            | Дата              | Последняя дата, когда пользователю была назначена Teams лицензия. |
| assignedProducts                  | Коллекция String | Все продукты, назначенные пользователю.  |

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


