---
title: Тип ресурса accessPackageResourceRoleScope
description: Область роли ресурса пакета доступа — это ссылка как на область в ресурсе, так и на роль в этом ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5c1446816f5487a579395f75dba521ba53f136fe
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272123"
---
# <a name="accesspackageresourcerolescope-resource-type"></a>Тип ресурса accessPackageResourceRoleScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В управлении правами [Azure AD](entitlementmanagement-root.md)область роли пакета доступа — это ссылка как на область в ресурсе, так и на роль в этом ресурсе для этой области.  Пакет доступа будет иметь доступ к области ролей пакета ресурсов для ресурсов в каталоге, которые имеют отношение к этому пакету доступа.  Когда субъект получает назначение пакета доступа, субъекту будет присвоена роль в этой области каждой области роли ресурса пакета доступа.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [Коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md) | Получить список объектов **accessPackageResourceRoleScope** для пакета доступа. |
| [Создание accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | Создайте новый **объект accessPackageResourceRoleScope** для пакета доступа. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdBy|String|Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String| Только для чтения.|
|modifiedBy|String|Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageResourceRole|[accessPackageResourceRole](accesspackageresourcerole.md)| Только для чтения. Допускается значение null.|
|accessPackageResourceScope|[accessPackageResourceScope](accesspackageresourcescope.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope",
  "keyProperty": "id"
}-->

```json
{
   "createdBy":"String",
   "createdDateTime":"String (timestamp)",
   "id":"String (identifier)",
   "modifiedBy":"String",
   "modifiedDateTime":"String (timestamp)",
   "accessPackageResourceRole":{
      "id":"String (identifier)",
      "displayName":"String",
      "originSystem":"String",
      "originId":"String"
   },
   "accessPackageResourceScope":{
      "id":"String (identifier)",
      "displayName":"String",
      "description":"String",
      "originId":"String (identifier)",
      "originSystem":"String"
   }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRoleScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


