---
title: тип ресурса unifiedRoleManagementPolicy
description: В unifiedRoleManagementPolicy указаны различные политики, связанные с областью и определением ролей. Она получена из microsoft.graph.policyBase.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 73510f928fa4a32e92ff0a50b3439ab60dfb95f8
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299665"
---
# <a name="unifiedrolemanagementpolicy-resource-type"></a>тип ресурса unifiedRoleManagementPolicy

Пространство имен: microsoft.graph

В unifiedRoleManagementPolicy указаны различные политики, связанные с областью и определением ролей. Она получена из microsoft.graph.policyBase.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список унифицированныхRoleManagementPolicies](../api/unifiedrolemanagementpolicy-list.md)|[коллекция unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Получите список объектов [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) и их свойств.|
|[Get unifiedRoleManagementPolicy](../api/unifiedrolemanagementpolicy-get.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleManagementPolicy.](../resources/unifiedrolemanagementpolicy.md)|
|[Список effectiveRules](../api/unifiedrolemanagementpolicy-list-effectiverules.md)|[коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Получите ресурсы unifiedRoleManagementPolicyRule из свойства эффективной навигацииRules.|
|[Список правил](../api/unifiedrolemanagementpolicy-list-rules.md)|[коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Получите ресурсы unifiedRoleManagementPolicyRule из свойства навигации правил.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|Строка|Описание политики.|
|displayName|Строка|Отображение имени политики.|
|id|Строка|Уникальный идентификатор для политики.|
|isOrganizationDefault|Логический|Это может быть установлено только для одной широкой политики клиента, которая будет применяться для всех областей и ролей. Установите область ScopeId на "/" и scopeType в Directory.|
|lastModifiedBy|[identity](../resources/identity.md)|Идентификатор, который в последний раз изменил параметр роли.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения параметра роли.|
|scopeId|Строка|ID области, в которой создается политика. Например, "/", groupId и т. д.|
|scopeType|Строка|Тип области, в которой создается политика. Один из Directory, DirectoryRole, Group.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|effectiveRules|[коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Список эффективных правил, таких как правило утверждения, правило истечения срока действия и т. д. оценивается на основе унаследованных ссылок. Например, Если существует широкая политика клиента по обеспечению соблюдения правила утверждения включения, эффективным правилом будет включение утверждения, даже если у полиса есть правило, чтобы отключить утверждение.|
|правила|[коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Коллекция правил, таких как правило утверждения, правило истечения срока действия и т. д.|

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

