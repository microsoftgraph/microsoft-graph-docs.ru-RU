---
title: Тип ресурса accessPackageResourceRole
description: Ссылка на роль, определенную в ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1d7f97410c924b804ef4002932ca75182a461989
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133604"
---
# <a name="accesspackageresourcerole-resource-type"></a>Тип ресурса accessPackageResourceRole

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении правами Azure AD](entitlementmanagement-root.md)роль ресурса пакета доступа является ссылкой на роль, определенную в ресурсе. Эта ссылка может использоваться после создания пакета доступа для указания ролей каждого из ресурсов каталога, в которые должен доставляться пакет доступа, путем создания области роли ресурса пакета [доступа.](../api/accesspackage-post-accesspackageresourcerolescopes.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список ролей ресурсов accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [Коллекция accessPackageResourceRole](accesspackageresourcerole.md) | Получить список объектов accessPackageResourceRole для каталога. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|Строка|Описание роли ресурса.|
|displayName|Строка|Отображаемого имени роли ресурса, например роли, определенной приложением.|
|id|String| Только для чтения.|
|originId|Строка|Уникальный идентификатор роли ресурса в системе источника. |
|originSystem|Строка|Тип ресурса в системе источника, например `SharePointOnline` , или `AadApplication` `AadGroup` .|

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
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "originId": "String",
  "originSystem": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


