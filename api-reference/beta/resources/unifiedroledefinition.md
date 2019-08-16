---
title: Тип ресурса Унифиедроледефинитион
description: Определение единой роли представляет собой коллекцию разрешений.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: be1b8a0b1a623c6cf322d5cf7997f04b87875c51
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437750"
---
# <a name="unifiedroledefinition-resource-type"></a>Тип ресурса Унифиедроледефинитион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Унифиедроледефинитион — это коллекция разрешений, в которой перечислены операции, которые можно выполнить, например чтение, запись и удаление.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Унифиедроледефинитион](../api/rbacapplication-list-roledefinitions.md) | Коллекция [унифиедроледефинитион](unifiedroledefinition.md) | Чтение списка объектов Унифиедроледефинитион и их свойств. |
| [Получение Унифиедроледефинитион](../api/unifiedroledefinition-get.md) | [унифиедроледефинитион](unifiedroledefinition.md) | Чтение свойств объекта Унифиедроледефинитион. |
| [Создание Унифиедроледефинитион](../api/rbacapplication-post-roledefinitions.md) | [унифиедроледефинитион](unifiedroledefinition.md) | Создание объекта Унифиедроледефинитион. |
| [Обновление Унифиедроледефинитион](../api/unifiedroledefinition-update.md) | [унифиедроледефинитион](unifiedroledefinition.md) | Обновление объекта Унифиедроледефинитион. |
| [Удаление Унифиедроледефинитион](../api/unifiedroledefinition-delete.md) | Нет | Удаление объекта Унифиедроледефинитион. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|String| Описание для Унифиедроледефинитион. Только для чтения, если для Builtin задано значение true. |
|displayName|Строка| Отображаемое имя для Унифиедроледефинитион. Только для чтения, если для Builtin задано значение true. Обязательный.|
|id|String| Уникальный идентификатор для Унифиедроледефинитион. Key, не допускающая значение null, только для чтения. |
|isBuiltIn|Boolean| Флаг, указывающий, является ли Унифиедроледефинитион частью набора по умолчанию, входящего в состав продукта или настраиваемого. Только для чтения. |
|isEnabled|Boolean| Флаг, указывающий, включена ли роль для назначения. Если значение false, роль недоступна для назначения. Только для чтения, если для Builtin задано значение true. |
|resourceScopes|Коллекция String| Список разрешений областей, к которым применяется определение роли. В настоящее время поддерживается только "/". Только для чтения, если для Builtin задано значение true. |
|rolePermissions|Коллекция [унифиедролепермиссион](unifiedrolepermission.md)| Список разрешений, включенных в роль. Только для чтения, если для Builtin задано значение true. Обязательно. |
|templateId|String| Настраиваемый идентификатор шаблона, который можно задать, если параметру Builtin присвоено значение false. Этот идентификатор обычно используется, если необходимо, чтобы один идентификатор совпадал для разных каталогов. Только для чтения, если для Builtin задано значение true. |
|version|String| Указывает версию Унифиедроледефинитион. Только для чтения, если для Builtin задано значение true.|

## <a name="relationships"></a>Отношения

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isBuiltIn": true,
  "isEnabled": true,
  "resourceScopes": ["String"],
  "rolePermissions": [{"@odata.type": "microsoft.graph.unifiedRolePermission"}],
  "templateId": "String",
  "version": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
