---
title: Тип ресурса office365ActiveUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 192629623b0a0d46453f4dd4f9bfd7f1dc48cccf
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575372"
---
# <a name="office365activeuserdetail-resource-type"></a>Тип ресурса office365ActiveUserDetail

## <a name="properties"></a>Свойства

| Свойство                          | Тип              | Описание                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| reportRefreshDate                 | Date              | Последняя дата контента.          |
| userPrincipalName                 | Строка            | Основной имя пользователя (UPN) пользователя. Имя участника-пользователя — это имя для входа характерном для Интернета для пользователя на основании Интернета standard RFC 822. В соответствии с соглашением это сопоставление имен пользователей электронной почты. Общие имеет формат alias@domain, где должны быть представлены в семейство подтвержденным доменов из домена. Это свойство обязательно указывать при создании пользователя. |
| displayName                       | String            | Имя пользователя, отображаемое в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. |
| isDeleted                         | Boolean           | Был ли этот пользователь удаленного или программных удалены. |
| deletedDate                       | Date              | Дата, когда произошло операцию удаления. Значение по умолчанию — значение «null», когда пользователь не были удалены. |
| hasExchangeLicense                | Boolean           | Является ли пользователь назначена лицензия Exchange. |
| hasOneDriveLicense                | Boolean           | Является ли пользователь был назначен OneDrive лицензии. |
| hasSharePointLicense              | Boolean           | Является ли пользователь был назначен лицензией SharePoint. |
| hasSkypeForBusinessLicense        | Boolean           | Является ли пользователь был назначен Скайп для корпоративную лицензию. |
| hasYammerLicense                  | Boolean           | Является ли пользователь была назначена лицензия Yammer. |
| hasTeamsLicense                   | Boolean           | Является ли пользователь назначена лицензия групп. |
| exchangeLastActivityDate          | Date              | Дата пользователя последняя чтения или отправки электронной почты. |
| oneDriveLastActivityDate          | Date              | Дата, когда пользователь последнего просмотра и редактирования файлов, общих файлов во внутреннем или внешнем ресурсе или синхронизирован файлы. |
| sharePointLastActivityDate        | Date              | Дату, когда пользователь последнего просмотра и редактирования файлов, общих файлов во внутренней сети или извне, синхронизированные файлы или просматривать страницы в SharePoint. |
| skypeForBusinessLastActivityDate  | Date              | Дата пользователя последнего упорядоченные или принявших участие в конференциях или в состав peer-to-peer sessions. |
| yammerLastActivityDate            | Date              | Дата пользователя последнего учета, чтение или нравится, что сообщение. |
| teamsLastActivityDate             | Date              | Дату, когда пользователь последнего учтены сообщения по каналам группы отправленных сообщений в сеансах частной беседы или являлся участником собрания и для вызовов. |
| exchangeLicenseAssignDate         | Date              | Последняя дата, когда пользователь была назначена лицензия Exchange. |
| oneDriveLicenseAssignDate         | Date              | Последняя дата, когда пользователь была назначена лицензия OneDrive. |
| sharePointLicenseAssignDate       | Date              | Последняя дата, когда пользователь была назначена лицензия SharePoint. |
| skypeForBusinessLicenseAssignDate | Date              | Последняя дата, когда пользователь была назначена лицензия Скайп для бизнеса. |
| yammerLicenseAssignDate           | Date              | Последняя дата, когда пользователь была назначена лицензия Yammer. |
| teamsLicenseAssignDate            | Date              | Последняя дата, когда пользователь была назначена лицензия группами. |
| assignedProducts                  | Коллекция String | Все продукты, назначенные для пользователя.  |

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
