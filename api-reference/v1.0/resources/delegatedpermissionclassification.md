---
title: тип ресурса delegatedPermissionClassification
description: Используется для указания классификации делегированного разрешения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: ff9f4ca394e2065c69fd7cd08a19d60817fc4f99
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761760"
---
# <a name="delegatedpermissionclassification-resource-type"></a>тип ресурса delegatedPermissionClassification

Пространство имен: microsoft.graph

Используется для указания классификации делегированного разрешения.

Делегированная классификация разрешений может использоваться в сочетании с настройками согласия пользователя для выбора разрешений, на которые разрешено согласие пользователя. Подробнее о классификации разрешений см. в приложении Configure how [end-users consent to applications.](/azure/active-directory/manage-apps/configure-user-consent)

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| id | String | Уникальный идентификатор для ключа **делегированияPermissionClassification.** Значение null не допускается. Только для чтения. |
| classification | permissionClassificationType | Задано значение классификации. Возможное значение: `low` . Не поддерживает `$filter`. |
| permissionId | Guid | Уникальный идентификатор **(id)** для делегированного разрешения, перечисленного в **коллекции oauth2PermissionScopes** [службыPrincipal.](servicePrincipal.md) Требуется при создании. Не поддерживает `$filter`. |
| permissionName | String | Значение утверждения **(значение)** для делегированного разрешения, перечисленного в **коллекции oauth2PermissionScopes** [службыPrincipal.](servicePrincipal.md) Не поддерживает `$filter`. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.delegatedPermissionClassification"
}-->

```json
{
  "id": "string (identifier)",
  "classification": "low",
  "permissionId": "string",
  "permissionName": "string"
}
```
