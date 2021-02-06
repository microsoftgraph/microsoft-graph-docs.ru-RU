---
title: Тип ресурса delegatedPermissionClassification
description: Используется для указания классификации делегированного разрешения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 4a567696d2adf0cd2a53cc2eb4d193ec1e1c2855
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133639"
---
# <a name="delegatedpermissionclassification-resource-type"></a>Тип ресурса delegatedPermissionClassification

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для указания классификации делегированного разрешения.

Делегированную классификацию разрешений можно использовать в сочетании с настройками согласия пользователя, чтобы выбрать разрешения, на которые пользователь может дать согласие. См. ["Настройка согласия конечных пользователей на использование](/azure/active-directory/manage-apps/configure-user-consent) приложений для получения дополнительных данных о классификациях разрешений".

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| id | Строка | Уникальный идентификатор ключа **delegatedPermissionClassification.** Значение null не допускается. Только для чтения. |
| classification | permissionClassificationType | Заданный значение классификации. Возможное значение: `low` . Не поддерживает `$filter`. |
| permissionId | Guid | Уникальный идентификатор **(идентификатор)** делегированного разрешения, перечисленного в коллекции **publishedPermissionScopes** [servicePrincipal.](servicePrincipal.md) Требуется при создании. Не поддерживает `$filter`. |
| permissionName | Строка | Значение утверждения **(значение)** для делегированного разрешения, перечисленного в коллекции **publishedPermissionScopes** [servicePrincipal.](servicePrincipal.md) Не поддерживает `$filter`. |

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

