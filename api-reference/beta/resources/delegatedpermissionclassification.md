---
title: Тип ресурса Делегатедпермиссионклассификатион
description: Используется для указания классификации делегированного разрешения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: f41ea807859b11982283b2a9743d6167e99dac66
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433704"
---
# <a name="delegatedpermissionclassification-resource-type"></a>Тип ресурса Делегатедпермиссионклассификатион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для указания классификации делегированного разрешения.

Делегированные классификации разрешений можно использовать в сочетании с параметрами согласия пользователя для выбора разрешений, на которые пользователю разрешено согласие. Узнайте, [как конечные пользователи](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) могут узнать больше о классификациях разрешений для приложений.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| id | String | Уникальный идентификатор для ключа **делегатедпермиссионклассификатион** . Значение null не допускается. Только для чтения. |
| classification | пермиссионклассификатионтипе | Заданное значение классификации. Возможные значения: `low` . Не поддерживает `$filter`. |
| пермиссионид | Guid | Уникальный идентификатор (**ID**) для делегированного разрешения, указанного в коллекции **публишедпермиссионскопес** объекта [servicePrincipal](servicePrincipal.md). Требуется при создании. Не поддерживает `$filter`. |
| пермиссионнаме | String | Значение утверждения (**value**) для делегированного разрешения, указанного в коллекции **публишедпермиссионскопес** объекта [servicePrincipal](servicePrincipal.md). Не поддерживает `$filter`. |

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
