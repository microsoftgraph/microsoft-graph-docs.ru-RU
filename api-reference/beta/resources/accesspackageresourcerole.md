---
title: Тип ресурса Акцесспаккажересаурцероле
description: Ссылка на роль, определенную в ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4bc0a60043c9877b4c48a889f93fa48a852c3780
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319589"
---
# <a name="accesspackageresourcerole-resource-type"></a>Тип ресурса Акцесспаккажересаурцероле

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)роль ресурса пакета Access — это ссылка на роль, определенную в ресурсе. Эту ссылку можно использовать после создания пакета Access, чтобы указать роли каждого из ресурсов каталога, к которым должен предоставлять пакет Access, путем [создания области применения роли ресурса пакета Access](../api/accesspackage-post-accesspackageresourcerolescopes.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список ролей ресурсов Акцесспаккажекаталог](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | Коллекция [акцесспаккажересаурцероле](accesspackageresourcerole.md) | Получение списка объектов Акцесспаккажересаурцероле для каталога. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|String|Описание роли ресурса.|
|displayName|String|Отображаемое имя роли ресурса, например роль, определяемую приложением.|
|id|String| Только для чтения.|
|оригинид|String|Уникальный идентификатор роли ресурса в исходной системе. |
|оригинсистем|String|Тип ресурса в исходной системе, например `SharePointOnline` , `AadApplication` или `AadGroup` .|

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
