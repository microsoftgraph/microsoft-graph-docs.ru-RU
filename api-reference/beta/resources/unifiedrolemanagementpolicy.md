---
title: тип ресурса unifiedRoleManagementPolicy
description: В unifiedRoleManagementPolicy указаны различные политики, связанные с областью и определением ролей. Она получена из microsoft.graph.policyBase.
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4b64b5fc402bab0d549d60c1653e826d80fa0bbd
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63667955"
---
# <a name="unifiedrolemanagementpolicy-resource-type"></a>тип ресурса unifiedRoleManagementPolicy

Пространство имен: microsoft.graph

УнифицированнаяRoleManagementPolicy указывает различные политики, связанные с областью Azure AD и определением ролей. Она получена из [сущности](entity.md). Для политик, применимых к Azure RBAC, используйте [API PIM REST Azure для политик управления ролью](/rest/api/authorization/role-management-policies).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список унифицированныхRoleManagementPolicies](../api/unifiedrolemanagementpolicy-list.md)|[коллекция unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Получите список объектов [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) и их свойств.|
|[Get unifiedRoleManagementPolicy](../api/unifiedrolemanagementpolicy-get.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) с учетом области.|
|[Список правил](../api/unifiedrolemanagementpolicy-list-rules.md)|[коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Получите ресурсы unifiedRoleManagementPolicyRule из свойства навигации правил.|
|[Получить правила](../api/unifiedrolemanagementpolicyrule-get.md)|[коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Получите правила для единого объектаRoleManagementPolicyRule.|
|[Обновление правил](../api/unifiedrolemanagementpolicyrule-update.md)|[коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Обнови правила для единого объектаRoleManagementPolicyRule.|
<!--unsurface effectiveRules because it hasn't been implemented
|[List effectiveRules](../api/unifiedrolemanagementpolicy-list-effectiverules.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection|Get the unifiedRoleManagementPolicyRule resources from the effectiveRules navigation property.|
-->

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|Строка|Описание политики.|
|displayName|Строка|Отображение имени политики.|
|id|String|Уникальный идентификатор для политики.|
|isOrganizationDefault|Boolean|Это может быть установлено только для одной широкой политики клиента, которая будет применяться для всех областей и ролей. Установите область ScopeId на "/" и scopeType в Directory.|
|lastModifiedBy|[identity](../resources/identity.md)|Идентификатор, который в последний раз изменил параметр роли.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения параметра роли.|
|scopeId|Строка|ID области, в которой создается политика. Может быть `/` для клиента или группового ИД. Обязательный.|
|scopeType|String|Тип области, в которой создается политика. Один из `Directory`. `DirectoryRole` Обязательный.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|effectiveRules|[коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|**Не реализовано.** Список эффективных правил, таких как правила утверждения и правила истечения срока действия, оцениваемого на основе унаследованных ссылок. Например, если существует политика, направленная на обеспечение соблюдения правила утверждения для клиента, эффективным правилом будет включение утверждения, даже если у политики есть правило отключения утверждения.|
|правила|[коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Коллекция правил, таких как правила утверждения и правила истечения срока действия.|

## <a name="json-representation"></a>Представление JSON
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

