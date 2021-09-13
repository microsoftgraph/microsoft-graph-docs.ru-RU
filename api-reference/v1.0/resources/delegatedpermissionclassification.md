---
title: тип ресурса delegatedPermissionClassification
description: Используется для указания классификации делегированного разрешения.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 088fd0264abebaec5e4bf4d9af14bbb4031de1e4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118752"
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
