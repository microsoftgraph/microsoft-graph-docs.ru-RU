---
title: Тип ресурса unifiedRoleManagementPolicyAuthenticationContextRule
description: Тип, производный от типа ресурса unifiedRoleManagementPolicyRule, который определяет правило контекста проверки подлинности для политики условного доступа, связанной с политикой управления ролем.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 118f24e9b449dbe2b1b8069741cea26e7f032990
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900452"
---
# <a name="unifiedrolemanagementpolicyauthenticationcontextrule-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyAuthenticationContextRule

Пространство имен: microsoft.graph

Тип, производный от типа ресурса [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) , который определяет правило контекста проверки подлинности для политики условного доступа, связанной с политикой управления ролем.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|claimValue|Строка|Значение утверждения контекста проверки подлинности.|
|id|Строка|Идентификатор правила. Наследуется от [сущности](../resources/entity.md).|
|isEnabled|Boolean| Указывает, включено ли это правило.|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Определяет сведения о области, предназначенной для правила включения. Сведения могут включать тип субъекта, тип назначения роли и действия, влияющие на роль. Наследуется [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md). Поддерживает `$filter` (`eq`, `ne`).|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "isEnabled": "Boolean",
  "claimValue": "String"
}
```

