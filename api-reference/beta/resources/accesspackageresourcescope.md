---
title: тип ресурса accessPackageResourceScope
description: В управлении правами Azure AD область ресурсов пакета доступа является ссылкой на область в ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6da0211cad6dcca225f4c9848216eda2deaf7b0a
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467178"
---
# <a name="accesspackageresourcescope-resource-type"></a>тип ресурса accessPackageResourceScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В управлении правами [Azure AD](entitlementmanagement-root.md)область ресурсов пакета доступа является ссылкой на область в ресурсе для тех ресурсов, которые имеют несколько областей.

Область ресурсов пакета доступа для ресурса, который уже добавлен в пакет доступа, можно определить с помощью списка [accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) для возврата коллекции объектов [accessPackageResourceRoleScope.](accesspackageresourcerolescope.md)

Если ресурс находится в каталоге пакетов доступа, но его роли еще не добавлены в пакет доступа, можно определить область ресурсов пакета доступа с помощью списка [accessPackageResources](../api/accesspackagecatalog-list-accesspackageresources.md) и в том числе в `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` запросе.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|String|Описание области.|
|displayName|String|Имя отображения области.|
|id|String| Только для чтения.|
|isRootScope|Логический|Верно, если области расположены в иерархии и это верхняя или корневая область ресурса.|
|OriginId|String|Уникальный идентификатор области в ресурсе, как определено в системе происхождения.|
|originSystem|String|Система происхождения для области.|
|roleOriginId|String|Система происхождения для роли, если отличается.|
|url|String|Локатор ресурсов для области.|

## <a name="relationships"></a>Связи

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


