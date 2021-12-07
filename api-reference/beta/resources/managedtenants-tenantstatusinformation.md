---
title: тип ресурса tenantStatusInformation
description: Представляет сведения о состоянии на борту для управляемого клиента.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 4d5cf90ebcb1567a84c4d7e0f00547f0e946598d
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61321969"
---
# <a name="tenantstatusinformation-resource-type"></a>тип ресурса tenantStatusInformation

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о состоянии на борту для управляемого клиента.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|delegatedPrivilegeStatus|delegatedPrivilegeStatus|Состояние отношения привилегий делегирования администратора между управляющей организацией и управляемым клиентом. Возможные значения: `none`, `delegatedAdminPrivileges`, `unknownFutureValue`. Необязательно. Только для чтения.|
|lastDelegatedPrivilegeRefreshDateTime|DateTimeOffset|Дата и время обновления статуса делегирования привилегий администратора. Необязательно. Только для чтения.|
|offboardedByUserId|Строка|Идентификатор учетной записи, которая отключалась от управляемого клиента. Необязательно. Только для чтения.|
|offboardedDateTime|DateTimeOffset|Дата и время отключения управляемого клиента. Необязательно. Только для чтения.|
|onboardedByUserId|Строка|Идентификатор учетной записи, в которую вошел управляемый клиент. Необязательно. Только для чтения.|
|onboardedDateTime|DateTimeOffset|Дата и время, когда управляемый клиент был на борту. Необязательно. Только для чтения.|
|onboardingStatus|tenantOnboardingStatus|Состояние onboarding для управляемого клиента.. Возможные значения: `ineligible`, `inProcess`, `active`, `inactive`, `unknownFutureValue`. Необязательно. Только для чтения.|
|tenantOnboardingEligibilityReason|tenantOnboardingEligibilityReason|Причина, по которой организация имеет право на участие в Microsoft 365 Lighthouse.. Возможные значения: `none` `contractType` , , , , `delegatedAdminPrivileges` и `usersCount` `license` `unknownFutureValue` . Необязательно. Только для чтения.|
|workloadStatuses|[коллекция microsoft.graph.managedTenants.workloadStatus](../resources/managedtenants-workloadstatus.md)|Коллекция статуй рабочей нагрузки для управляемого клиента. Необязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantStatusInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantStatusInformation",
  "onboardingStatus": "String",
  "onboardedDateTime": "String (timestamp)",
  "onboardedByUserId": "String",
  "offboardedDateTime": "String (timestamp)",
  "offboardedByUserId": "String",
  "delegatedPrivilegeStatus": "String",
  "lastDelegatedPrivilegeRefreshDateTime": "String (timestamp)",
  "workloadStatuses": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadStatus"
    }
  ]
}
```
