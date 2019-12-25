---
title: Тип ресурса Акцесспаккажересаурцескопе
description: В управлении службой управления правами Azure AD областью ресурсов пакета Access является ссылка на область в пределах ресурса.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1418e2cb21a1023e864d842b760006e05f3afb03
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870969"
---
# <a name="accesspackageresourcescope-resource-type"></a>Тип ресурса Акцесспаккажересаурцескопе

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)область ресурсов пакета Access — это ссылка на область в ресурсе для этих ресурсов с несколькими областями.

Можно определить область ресурсов пакета доступа для ресурса, который уже был добавлен в пакет Access, с помощью [List акцесспаккажересаурцеролескопес](../api/accesspackage-list-accesspackageresourcerolescopes.md) , чтобы вернуть коллекцию объектов [акцесспаккажересаурцеролескопе](accesspackageresourcerolescope.md) .

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|String|Описание области.|
|displayName|Строка|Отображаемое имя области.|
|id|String| Только для чтения.|
|исрутскопе|Логический|Значение true, если области упорядочены в иерархию, а это верхняя или корневая область ресурса.|
|оригинид|String|Уникальный идентификатор области ресурса в соответствии с определением в исходной системе.|
|оригинсистем|String|Исходная система для области.|
|ролеоригинид|String|Исходная система для роли, если она отличается.|
|url|String|Указатель ресурсов для области.|

## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|акцесспаккажересаурце|[акцесспаккажересаурце](accesspackageresource.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceScope",
  "baseType": "",
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
