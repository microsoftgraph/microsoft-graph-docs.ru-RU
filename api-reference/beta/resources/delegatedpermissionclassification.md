---
title: тип ресурса delegatedPermissionClassification
description: Используется для указания классификации делегированного разрешения.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 72cc4630ba8f28fe0d76722178edcdd3ffed5943
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854645"
---
# <a name="delegatedpermissionclassification-resource-type"></a>тип ресурса delegatedPermissionClassification

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для указания классификации делегированного разрешения.

Делегированная классификация разрешений может использоваться в сочетании с настройками согласия пользователя для выбора разрешений, на которые разрешено согласие пользователя. Подробнее о классификации разрешений см. в приложении [Configure how end-users consent to applications](/azure/active-directory/manage-apps/configure-user-consent) .

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| id | String | Уникальный идентификатор для ключа **делегированияPermissionClassification** . Значение null не допускается. Только для чтения. |
| classification | permissionClassificationType | Задано значение классификации. Возможное значение: `low`. Не поддерживает `$filter`. |
| permissionId | GUID | Уникальный идентификатор (**идентификатор**) для делегированного разрешения, перечисленного в опубликованной **коллекцииPermissionScopes** [службыPrincipal](servicePrincipal.md). Требуется при создании. Не поддерживает `$filter`. |
| permissionName | String | Значение утверждения (**значение**) для делегированного разрешения, перечисленного в опубликованной **коллекцииPermissionScopes** [службыPrincipal](servicePrincipal.md). Не поддерживает `$filter`. |

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

