---
title: тип ресурса operationApprovalPolicySet
description: Содержит пару OperationApprovalPolicyType и OperationApprovalPolicyPlatform, определяющих набор применимых operationApprovalPolicies для пользователя
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 54ba00c62c6618d10dbc81cfc9587a4204f0f368
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2021
ms.locfileid: "60493817"
---
# <a name="operationapprovalpolicyset-resource-type"></a>тип ресурса operationApprovalPolicySet

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит пару OperationApprovalPolicyType и OperationApprovalPolicyPlatform, определяющих набор применимых operationApprovalPolicies для пользователя

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|policyType|[operationApprovalPolicyType](../resources/intune-rbac-operationapprovalpolicytype.md)|Тип политики для этой операцииApprovalPolicy. Это свойство доступно только для чтения. Возможные значения: `deviceActions` `deviceWipe` , , , , , `deviceRetire` , , , `deviceRetireNonCompliant` `deviceDelete` , , `deviceLock` `deviceErase` `deviceDisableActivationLock` `windowsEnrollment` , `compliancePolicies` `configurationPolicies` `appProtectionPolicies` `policySets` `filters` `endpointSecurity` `apps` `scripts` `roles` `unknownFutureValue` .|
|policyPlatform|[operationApprovalPolicyPlatform](../resources/intune-rbac-operationapprovalpolicyplatform.md)|Применимая платформа (ы) для этой ОперацииApprovalPolicy. Это свойство доступно только для чтения. Возможные значения: `notApplicable`, `androidDeviceAdministrator`, `androidEnterprise`, `iOSiPadOS`, `macOS`, `windows10AndLater`, `windows81AndLater`, `windows10X`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationApprovalPolicySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operationApprovalPolicySet",
  "policyType": "String",
  "policyPlatform": "String"
}
```



