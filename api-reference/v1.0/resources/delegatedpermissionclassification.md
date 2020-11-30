---
title: Тип ресурса Делегатедпермиссионклассификатион
description: Используется для указания классификации делегированного разрешения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 7d5926bff0d7096080aa22fae49d0ed15c7d1fcd
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377419"
---
# <a name="delegatedpermissionclassification-resource-type"></a>Тип ресурса Делегатедпермиссионклассификатион

Пространство имен: microsoft.graph

Используется для указания классификации делегированного разрешения.

Делегированные классификации разрешений можно использовать в сочетании с параметрами согласия пользователя для выбора разрешений, на которые пользователю разрешено согласие. Узнайте, [как конечные пользователи](/azure/active-directory/manage-apps/configure-user-consent) могут узнать больше о классификациях разрешений для приложений.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| id | Строка | Уникальный идентификатор для ключа **делегатедпермиссионклассификатион** . Значение null не допускается. Только для чтения. |
| classification | пермиссионклассификатионтипе | Заданное значение классификации. Возможные значения: `low` . Не поддерживает `$filter`. |
| пермиссионид | Guid | Уникальный идентификатор (**ID**) для делегированного разрешения, указанного в коллекции **oauth2PermissionScopes** объекта [servicePrincipal](servicePrincipal.md). Требуется при создании. Не поддерживает `$filter`. |
| пермиссионнаме | Строка | Значение утверждения (**value**) для делегированного разрешения, указанного в коллекции **oauth2PermissionScopes** объекта [servicePrincipal](servicePrincipal.md). Не поддерживает `$filter`. |

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
