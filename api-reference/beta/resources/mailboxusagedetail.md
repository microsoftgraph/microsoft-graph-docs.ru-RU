---
title: Тип ресурса mailboxUsageDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 63b4b997a0ae559338fffd2acfabaa35dcc306e0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938736"
---
# <a name="mailboxusagedetail-resource-type"></a>Тип ресурса mailboxUsageDetail

## <a name="properties"></a>Свойства

| Свойство                        | Тип    |
| :------------------------------ | :------ |
| reportRefreshDate               | Date    |
| userPrincipalName               | String  |
| displayName                     | String  |
| isDeleted                       | Boolean |
| deletedDate                     | Date    |
| Дата создания                     | Date    |
| lastActivityDate                | Date    |
| itemCount                       | Int64   |
| storageUsedInBytes              | Int64   |
| issueWarningQuotaInBytes        | Int64   |
| prohibitSendQuotaInBytes        | Int64   |
| prohibitSendReceiveQuotaInBytes | Int64   |
| reportPeriod                    | String  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "createdDate": "Date", 
  "lastActivityDate": "Date", 
  "itemCount": 1024, 
  "storageUsedInBytes": 1024, 
  "issueWarningQuotaInBytes": 1024, 
  "prohibitSendQuotaInBytes": 1024, 
  "prohibitSendReceiveQuotaInBytes": 1024, 
  "reportPeriod": "String"
}
```
