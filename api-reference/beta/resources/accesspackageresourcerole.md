---
title: тип ресурса accessPackageResourceRole
description: Ссылка на роль, определенную в ресурсе.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5652e9c867b235bc87cf67584056ce4425f1da80
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651191"
---
# <a name="accesspackageresourcerole-resource-type"></a>тип ресурса accessPackageResourceRole

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении правами Azure AD](entitlementmanagement-overview.md)роль ресурса пакета доступа является ссылкой на роль, определенную в ресурсе. Эта ссылка может быть использована после создания пакета доступа для указания ролей каждого из ресурсов каталога, в которые должен доставить пакет доступа, путем создания области ролей ресурсов пакета [доступа.](../api/accesspackage-post-accesspackageresourcerolescopes.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Роли ресурсов accessPackageCatalog в списке](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [коллекция accessPackageResourceRole](accesspackageresourcerole.md) | Извлечение списка объектов accessPackageResourceRole для каталога. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|Строка|Описание роли ресурса.|
|displayName|Строка|Отображение имени роли ресурса, например роли, определенной приложением.|
|id|String| Только для чтения.|
|OriginId|Строка|Уникальный идентификатор роли ресурса в системе происхождения. Для сайта SharePoint Online originId будет номером последовательности роли на сайте. |
|originSystem|String|Тип ресурса в системе происхождения, например `SharePointOnline` , `AadApplication` или `AadGroup` .|

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
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
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


