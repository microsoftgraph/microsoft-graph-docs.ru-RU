---
title: Тип ресурса operationApprovalPolicy
description: Политика утверждения операций
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 45076a2f7b7e4354a7df06182904887c1147ecaa
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211307"
---
# <a name="operationapprovalpolicy-resource-type"></a>Тип ресурса operationApprovalPolicy

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политика утверждения операций

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление operationApprovalPolicies](../api/intune-rbac-operationapprovalpolicy-list.md)|[Коллекция operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Список свойств и связей объектов [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) .|
|[Получение operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-get.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Чтение свойств и связей объекта [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) .|
|[Создание operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-create.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Создайте объект [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) .|
|[Удаление operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-delete.md)|Нет|Удаляет [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md).|
|[Обновление operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-update.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Обновление свойств объекта [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) .|
|[Функция getApprovableOperations](../api/intune-rbac-operationapprovalpolicy-getapprovableoperations.md)|[Коллекция operationApprovalPolicySet](../resources/intune-rbac-operationapprovalpolicyset.md)|Пока не задокументировано.|
|[Функция getOperationsRequiringApproval](../api/intune-rbac-operationapprovalpolicy-getoperationsrequiringapproval.md)|[Коллекция operationApprovalPolicySet](../resources/intune-rbac-operationapprovalpolicyset.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор OperationApprovalPolicy. Это свойство доступно только для чтения.|
|displayName|Строка|Отображаемое имя объекта OperationApprovalPolicy|
|description|Строка|Описание этой политики OperationApprovalPolicy|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения этой политики OperationApprovalPolicy. Это свойство доступно только для чтения.|
|policyType|[operationApprovalPolicyType](../resources/intune-rbac-operationapprovalpolicytype.md)|Тип политики для этой политики OperationApprovalPolicy. Возможные значения: `deviceActions`, , `deviceWipe``deviceRetire`, , `deviceRetireNonCompliant`, `deviceDelete`, `deviceLock``deviceErase`, `deviceDisableActivationLock`, `compliancePolicies``windowsEnrollment`, `configurationPolicies`, `appProtectionPolicies`, , `policySets`, `filters`, `endpointSecurity`, `apps`, , `scripts`, , `roles`, , `deviceResetPasscode``unknownFutureValue`.|
|approverGroupIds|Коллекция строк|Идентификаторы групп для утверждающих для этой политики OperationApprovalPolicy|

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
  "approverGroupIds": [
    "String"
  ]
}
```




