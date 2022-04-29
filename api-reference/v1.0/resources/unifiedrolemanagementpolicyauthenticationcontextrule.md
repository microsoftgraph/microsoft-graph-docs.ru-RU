---
title: Тип ресурса unifiedRoleManagementPolicyAuthenticationContextRule
description: Тип, производный от типа ресурса unifiedRoleManagementPolicyRule, который определяет правило контекста проверки подлинности для политики условного доступа, связанной с политикой управления ролем.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3c0b14599cff017b97ce0f40e7c508a4d31cdc83
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134360"
---
# <a name="unifiedrolemanagementpolicyauthenticationcontextrule-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyAuthenticationContextRule

Пространство имен: microsoft.graph

Тип, производный от типа ресурса [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) , который определяет правило контекста проверки подлинности для политики условного доступа, связанной с политикой управления ролем.

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|claimValue|String|Значение утверждения контекста проверки подлинности.|
|id|String|Идентификатор правила. Наследуется от [сущности](../resources/entity.md).|
|isEnabled|Boolean| Указывает, включено ли это правило.|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Определяет сведения о области, предназначенной для правила включения. Сведения могут включать тип субъекта, тип назначения роли и действия, влияющие на роль. Наследуется [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md). Поддерживает `$filter` (`eq`, `ne`).|

## <a name="relationships"></a>Связи
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

