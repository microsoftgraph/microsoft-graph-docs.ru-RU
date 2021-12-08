---
title: тип ресурса operationApprovalPolicySet
description: Содержит пару OperationApprovalPolicyType и OperationApprovalPolicyPlatform, определяющих набор применимых operationApprovalPolicies для пользователя
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d314a9ca5d8f842b7e898ba0ff358241bf996e2f
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61340174"
---
# <a name="operationapprovalpolicyset-resource-type"></a>тип ресурса operationApprovalPolicySet

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит пару OperationApprovalPolicyType и OperationApprovalPolicyPlatform, определяющих набор применимых operationApprovalPolicies для пользователя

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|policyType|[operationApprovalPolicyType](../resources/intune-rbac-operationapprovalpolicytype.md)|Тип политики для этой операцииApprovalPolicy. Это свойство доступно только для чтения. Возможные значения: `deviceActions` `deviceWipe` , , , , , `deviceRetire` `deviceRetireNonCompliant` , `deviceDelete` `deviceLock` `deviceErase` `deviceDisableActivationLock` `windowsEnrollment` `compliancePolicies` , `configurationPolicies` `appProtectionPolicies` `policySets` `filters` `endpointSecurity` `apps` `scripts` `roles` `deviceResetPasscode` `unknownFutureValue` .|
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




