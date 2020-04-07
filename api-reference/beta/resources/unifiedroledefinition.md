---
title: Тип ресурса Унифиедроледефинитион
description: Определение единой роли представляет собой коллекцию разрешений.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 76b5becc6ad8cec4a7e917ec20bcc58271ab797a
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160228"
---
# <a name="unifiedroledefinition-resource-type"></a>Тип ресурса Унифиедроледефинитион

Пространство имен: microsoft.graph

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
|id|Строка| Уникальный идентификатор для Унифиедроледефинитион. Key, не допускающая значение null, только для чтения. |
|isBuiltIn|Логический| Флаг, указывающий, является ли Унифиедроледефинитион частью набора по умолчанию, входящего в состав продукта или настраиваемого. Только для чтения. |
|isEnabled|Boolean| Флаг, указывающий, включена ли роль для назначения. Если значение false, роль недоступна для назначения. Только для чтения, если для Builtin задано значение true. |
|resourceScopes|Коллекция String| Список разрешений областей, к которым применяется определение роли. В настоящее время поддерживается только "/". Только для чтения, если для Builtin задано значение true. **НЕ ИСПОЛЬЗУЙТЕ. Это скоро будет рекомендуемым. Присоединение области к назначению роли** | 
|rolePermissions|Коллекция [унифиедролепермиссион](unifiedrolepermission.md)| Список разрешений, включенных в роль. Только для чтения, если для Builtin задано значение true. Обязательно. |
|templateId|Строка| Настраиваемый идентификатор шаблона, который можно задать, если параметру Builtin присвоено значение false. Этот идентификатор обычно используется, если необходимо, чтобы один идентификатор совпадал для разных каталогов. Только для чтения, если для Builtin задано значение true. |
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