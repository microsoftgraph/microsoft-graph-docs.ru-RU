---
title: тип ресурса accessPackageAssignmentRequestRequirements
description: Определяет требования, необходимые для запроса указанного пакета доступа.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 96179dd106936d5f39d5636231788ad51837473e
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242727"
---
# <a name="accesspackageassignmentrequestrequirements-resource-type"></a>тип ресурса accessPackageAssignmentRequestRequirements

Пространство имен: microsoft.graph

Представляет требования, которые должен выполнить звонячий для успешного создания **accessPackageAssignmentRequest** для **accessPackage,** указанного в URL-адресе. Требования определяются путем оценки политик, связанных с **accessPackage.** 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowCustomAssignmentSchedule|Boolean|Указывает, разрешено ли запрашивать для настройки настраиваемой расписания.|
|isApprovalRequiredForAdd|Boolean|Указывает, должен ли одобрение запроса на добавление.|
|isApprovalRequiredForUpdate|Boolean|Указывает, должен ли одобритель утверждать запрос на обновление.|
|policyDescription|Строка|Описание политики, с помощью которую пользователь пытается запрашивать доступ.|
|policyDisplayName|Строка|Отображает имя политики, с помощью которого пользователь пытается запрашивать доступ.|
|policyId|Строка|Идентификатор политики, с которую связаны эти требования. Этот идентификатор можно использовать при создании нового запроса на назначение.|
|schedule|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|Расписание введенных ограничений, если таковые есть.|

## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequestRequirements"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequestRequirements",
  "policyId": "String",
  "policyDisplayName": "String",
  "policyDescription": "String",
  "isApprovalRequiredForAdd": "Boolean",
  "isApprovalRequiredForUpdate": "Boolean",
  "allowCustomAssignmentSchedule": "Boolean",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  }
}
```


