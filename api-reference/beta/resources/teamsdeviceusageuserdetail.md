---
title: тип ресурса teamsDeviceUsageUserDetail
description: Представляет сведения об использовании устройства Microsoft Teams пользователем.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 294ffee8a1a5db208508cce230377285d6834b07
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766058"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a>тип ресурса teamsDeviceUsageUserDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об использовании устройства Microsoft Teams пользователем.

## <a name="properties"></a>Свойства

| Свойство          | Тип    | Описание                                                  |
| :---------------- | :------ | ------------------------------------------------------------ |
| reportRefreshDate | Дата    | Последняя дата контента.                              |
| userPrincipalName | String  | Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. |
| isLicensed        | Логический | Назначена ли пользователю лицензия Teams.          |
| lastActivityDate  | Дата    | Последняя дата участия пользователя в действии Microsoft Teams. |
| isDeleted         | Логический | Был ли этот пользователь удален или удален.          |
| deletedDate       | Дата    | Дата, когда произошла операция удаления. Значение по умолчанию — "null", если пользователь не удален. |
| usedWeb           | Логический | Был ли пользователь активен в веб-клиенте Teams на устройствах. |
| usedWindowsPhone  | Логический | Был ли пользователь активен в мобильном клиенте Teams для windows phone. |
| usediOS           | Логический | Был ли пользователь активен в мобильном клиенте Teams для iOS. |
| usedMac           | Логический | Был ли пользователь активен в настольном клиенте Teams на компьютере macOS. |
| usedAndroidPhone  | Логический | Был ли пользователь активен в мобильном клиенте Teams для Android. |
| usedWindows       | Логический | Был ли пользователь активен в настольном клиенте Teams на компьютере с Windows. |
| usedChromeOS      | Логический | Был ли пользователь активен в настольном клиенте Teams на компьютере ChromeOS. |
| usedLinux         | Логический | Был ли пользователь активен в настольном клиенте Teams на компьютере Linux. |
| reportPeriod      | String  | Количество дней, которые охватывает отчет.                        |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isLicensed": true, 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "usedChromeOS": true, 
  "usedLinux": true, 
  "reportPeriod": "String"
}
```


