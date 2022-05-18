---
title: Тип ресурса requestSchedule
description: В PIM используйте этот ресурс, чтобы определить расписание, в течение которых субъект будет иметь допустимую или активную роль.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 59adc6589ea351d565248797aeb9384b9ae3f890
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461445"
---
# <a name="requestschedule-resource-type"></a>Тип ресурса requestSchedule

Пространство имен: microsoft.graph

В PIM при создании или обновлении объекта [unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) или [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md) используйте этот ресурс для определения расписания назначения роли субъекту. Параметры, допустимые для этого объекта, зависят от [параметров Azure AD роли](../api/unifiedrolemanagementpolicy-list-rules.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Истечения срока действия|[expirationPattern](../resources/expirationpattern.md)|По истечении срока действия допустимого или активного назначения.|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|Частота допустимого или активного назначения. Это свойство в настоящее время не поддерживается в PIM.|
|startDateTime|DateTimeOffset|Когда допустимое или активное назначение становится активным.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.requestSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.requestSchedule",
  "startDateTime": "String (timestamp)",
  "expiration": {
    "@odata.type": "microsoft.graph.expirationPattern"
  },
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  }
}
```

