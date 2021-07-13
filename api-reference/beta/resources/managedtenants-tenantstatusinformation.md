---
title: тип ресурса tenantStatusInformation
description: Представляет сведения о состоянии на борту для управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 3e01ac003cda223788e0fc8e6dae01f18667da11
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402687"
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
|offboardedByUserId|String|Идентификатор учетной записи, которая отключалась от управляемого клиента. Необязательно. Только для чтения.|
|offboardedDateTime|DateTimeOffset|Дата и время отключения управляемого клиента. Необязательно. Только для чтения.|
|onboardedByUserId|String|Идентификатор учетной записи, в которую вошел управляемый клиент. Необязательно. Только для чтения.|
|onboardedDateTime|DateTimeOffset|Дата и время, когда управляемый клиент был на борту. Необязательно. Только для чтения.|
|onboardingStatus|tenantOnboardingStatus|Состояние onboarding для управляемого клиента.. Возможные значения: `ineligible`, `inProcess`, `active`, `inactive`, `unknownFutureValue`. Необязательно. Только для чтения.|
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
