---
title: Тип ресурса unifiedRoleManagementPolicy
description: Указывает различные политики, связанные с областями и ролями.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 95e068de21681735d2da1023452d57d11ed5ecf2
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437088"
---
# <a name="unifiedrolemanagementpolicy-resource-type"></a>Тип ресурса unifiedRoleManagementPolicy

Пространство имен: microsoft.graph

Указывает различные политики, связанные с областями и ролями. Для политик, применяемых к Azure RBAC, используйте [API REST PIM Azure для политик управления ролами](/rest/api/authorization/role-management-policies).

В настоящее время все политики и связанные правила доступны только для чтения.

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление unifiedRoleManagementPolicies](../api/policyroot-list-rolemanagementpolicies.md)|[Коллекция unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Получение политик управления ролами и их сведений.|
|[Получение unifiedRoleManagementPolicy](../api/unifiedrolemanagementpolicy-get.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Получение сведений о политике управления ролами.|
|[Список правил](../api/unifiedrolemanagementpolicy-list-rules.md)|[Коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Получение правил, определенных для политики управления ролем.|
|[Получение unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-get.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Получение правила, определенного для политики управления ролем.|
|[Обновление unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-update.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Обновление правила, определенного для политики управления ролем.|


## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|Описание политики.|
|displayName|String|Отображаемое имя политики.|
|id|String|Уникальный идентификатор политики.|
|isOrganizationDefault|Boolean|Это значение можно задать только `true` для одной политики на уровне клиента, которая будет применяться ко всем областям и ролям. Задайте для scopeId значение `/` и scopeType значение `Directory`. Поддерживает `$filter` (`eq`, `ne`).|
|lastModifiedBy|[identity](../resources/identity.md)|Удостоверение, который последним изменил параметр роли.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения параметра роли.|
|scopeId|String|Идентификатор области, в которой создается политика. Может быть `/` для клиента или идентификатора группы. Обязательный элемент.|
|scopeType|String|Тип области, в которой создается политика. Один из `Directory`, `DirectoryRole`. Обязательный.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|effectiveRules|[Коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)| Список действующих правил, таких как правила утверждения и правила срока действия, вычисляемые на основе наследуемых ссылочных правил. Например, если существует политика на уровне клиента для принудительного включения правила утверждения, эффективным правилом будет включение утверждения, даже если политика имеет правило для отключения утверждения. Поддерживает `$expand`.|
|правила|[Коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Коллекция правил, таких как правила утверждения и правила срока действия. Поддерживает `$expand`.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isOrganizationDefault": "Boolean",
  "scopeId": "String",
  "scopeType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identity"
  }
}
```

