---
title: Тип ресурса unifiedRoleManagementPolicy
description: UnifiedRoleManagementPolicy указывает различные политики, связанные с областью действия и определением роли. Он является производным от microsoft.graph.policyBase.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 39718aad157a43d68c2c0b3fce4f8c63ef128983
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398015"
---
# <a name="unifiedrolemanagementpolicy-resource-type"></a>Тип ресурса unifiedRoleManagementPolicy

Пространство имен: microsoft.graph

UnifiedRoleManagementPolicy указывает различные политики, связанные с Azure AD области и определения роли. Он является производным от [сущности](entity.md). Для политик, применяемых к Azure RBAC, используйте [API REST PIM Azure для политик управления ролами](/rest/api/authorization/role-management-policies).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление unifiedRoleManagementPolicies](../api/unifiedrolemanagementpolicy-list.md)|[Коллекция unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Получение списка объектов [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) и их свойств.|
|[Получение unifiedRoleManagementPolicy](../api/unifiedrolemanagementpolicy-get.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Чтение свойств и связей объекта [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) по заданной области.|
|[Список правил](../api/unifiedrolemanagementpolicy-list-rules.md)|[Коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Получите ресурсы unifiedRoleManagementPolicyRule из свойства навигации правил.|
|[Получение правил](../api/unifiedrolemanagementpolicyrule-get.md)|[Коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Получение правил для объекта unifiedRoleManagementPolicyRule.|
|[Обновление правил](../api/unifiedrolemanagementpolicyrule-update.md)|[Коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Обновите правила для объекта unifiedRoleManagementPolicyRule.|
<!--unsurface effectiveRules because it hasn't been implemented
|[List effectiveRules](../api/unifiedrolemanagementpolicy-list-effectiverules.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection|Get the unifiedRoleManagementPolicyRule resources from the effectiveRules navigation property.|
-->

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|Описание политики.|
|displayName|String|Отображаемое имя политики.|
|id|String|Уникальный идентификатор политики.|
|isOrganizationDefault|Логическое|Это значение можно задать только для одной политики на уровне клиента, которая будет применяться ко всем областям и ролям. Задайте для scopeId значение "/", а scopeType — каталог.|
|lastModifiedBy|[identity](../resources/identity.md)|Удостоверение, который последним изменил параметр роли.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения параметра роли.|
|scopeId|String|Идентификатор области, в которой создается политика. Может быть `/` для клиента или идентификатора группы. Обязательно.|
|scopeType|String|Тип области, в которой создается политика. Один из `Directory`, `DirectoryRole`. Обязательный.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|effectiveRules|[Коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|**Не реализовано.** Список действующих правил, таких как правила утверждения и правила срока действия, вычисляемые на основе наследуемых ссылочных правил. Например, если существует политика на уровне клиента для принудительного включения правила утверждения, эффективным правилом будет включение утверждения, даже если политика имеет правило для отключения утверждения.|
|правила|[Коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Коллекция правил, таких как правила утверждения и правила срока действия.|

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicy",
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

