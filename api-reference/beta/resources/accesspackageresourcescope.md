---
title: тип ресурса accessPackageResourceScope
description: В управлении правами Azure AD область ресурсов пакета доступа является ссылкой на область в ресурсе.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f403f6b2d7c88d1e24c579578c2c1b872bbbecdf
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651234"
---
# <a name="accesspackageresourcescope-resource-type"></a>тип ресурса accessPackageResourceScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В управлении правами [Azure AD](entitlementmanagement-overview.md)область ресурсов пакета доступа является ссылкой на область в ресурсе для тех ресурсов, которые имеют несколько областей.

Область ресурсов пакета доступа для ресурса, который уже добавлен в пакет доступа, можно определить с помощью списка [accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) для возврата коллекции объектов [accessPackageResourceRoleScope.](accesspackageresourcerolescope.md)

Если ресурс находится в каталоге пакетов доступа, но его роли еще не добавлены в пакет доступа, можно определить область ресурсов пакета доступа с помощью списка [accessPackageResources](../api/accesspackagecatalog-list-accesspackageresources.md) и в том числе в `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` запросе.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|Строка|Описание области.|
|displayName|Строка|Имя отображения области.|
|id|String| Только для чтения.|
|isRootScope|Boolean|Верно, если области расположены в иерархии и это верхняя или корневая область ресурса.|
|OriginId|Строка|Уникальный идентификатор области в ресурсе, как определено в системе происхождения.|
|originSystem|Строка|Система происхождения для области.|
|roleOriginId|Строка|Система происхождения для роли, если отличается.|
|url|String|Локатор ресурсов для области.|

## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageResource|[accessPackageResource](accesspackageresource.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceScope",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isRootScope": true,
  "originId": "String",
  "originSystem": "String",
  "roleOriginId": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


