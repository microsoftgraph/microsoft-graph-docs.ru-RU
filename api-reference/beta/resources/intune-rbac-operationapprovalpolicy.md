---
title: тип ресурса operationApprovalPolicy
description: Политика утверждения операции
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d2da950900e621d4f0a50b03c86c144d36dea412
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2021
ms.locfileid: "60487441"
---
# <a name="operationapprovalpolicy-resource-type"></a>тип ресурса operationApprovalPolicy

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политика утверждения операции

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список операцииApprovalPolicies](../api/intune-rbac-operationapprovalpolicy-list.md)|[коллекция operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Список свойств и связей объектов [operationApprovalPolicy.](../resources/intune-rbac-operationapprovalpolicy.md)|
|[Get operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-get.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Чтение свойств и связей объекта [operationApprovalPolicy.](../resources/intune-rbac-operationapprovalpolicy.md)|
|[Создание операцииApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-create.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Создайте новый [объект operationApprovalPolicy.](../resources/intune-rbac-operationapprovalpolicy.md)|
|[Удаление операцииApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-delete.md)|Нет|Удаляет [операциюApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md).|
|[Обновление операцииApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-update.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Обновление свойств объекта [operationApprovalPolicy.](../resources/intune-rbac-operationapprovalpolicy.md)|
|[функция getOperationsAllowedApproval](../api/intune-rbac-operationapprovalpolicy-getoperationsallowedapproval.md)|[коллекция operationApprovalPolicySet](../resources/intune-rbac-operationapprovalpolicyset.md)|Пока не задокументировано.|
|[функция getOperationsRequiringApproval](../api/intune-rbac-operationapprovalpolicy-getoperationsrequiringapproval.md)|[коллекция operationApprovalPolicySet](../resources/intune-rbac-operationapprovalpolicyset.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID операцииApprovalPolicy. Это свойство доступно только для чтения.|
|displayName|String|Имя отображения этой операцииApprovalPolicy|
|description|String|Описание этой операцииApprovalPolicy|
|lastModifiedDateTime|DateTimeOffset|Последняя измененная дата и время операцииApprovalPolicy. Это свойство доступно только для чтения.|
|policyType|[operationApprovalPolicyType](../resources/intune-rbac-operationapprovalpolicytype.md)|Тип политики для этой операцииApprovalPolicy. Возможные значения: `deviceActions` `deviceWipe` , , , , , `deviceRetire` , , , `deviceRetireNonCompliant` `deviceDelete` , , `deviceLock` `deviceErase` `deviceDisableActivationLock` `windowsEnrollment` , `compliancePolicies` `configurationPolicies` `appProtectionPolicies` `policySets` `filters` `endpointSecurity` `apps` `scripts` `roles` `unknownFutureValue` .|
|policyPlatform|[operationApprovalPolicyPlatform](../resources/intune-rbac-operationapprovalpolicyplatform.md)|Применимая платформа (ы) для этой ОперацииApprovalPolicy. Возможные значения: `notApplicable`, `androidDeviceAdministrator`, `androidEnterprise`, `iOSiPadOS`, `macOS`, `windows10AndLater`, `windows81AndLater`, `windows10X`.|
|approverGroupIds|Коллекция строк|Групповые ID для тех, кто одобряет эту операциюApprovalPolicy|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.operationApprovalPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operationApprovalPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "policyType": "String",
  "policyPlatform": "String",
  "approverGroupIds": [
    "String"
  ]
}
```



