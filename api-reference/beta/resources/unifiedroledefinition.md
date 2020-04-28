---
title: Тип ресурса Унифиедроледефинитион
description: Определение единой роли представляет собой коллекцию разрешений.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fd26a0526327c4b630f52fd80d5a75b4df9430c7
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218025"
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
|id|String| Уникальный идентификатор для Унифиедроледефинитион. Key, не допускающая значение null, только для чтения. |
|isBuiltIn|Boolean| Флаг, указывающий, является ли Унифиедроледефинитион частью набора по умолчанию, входящего в состав продукта или настраиваемого. Только для чтения. |
|isEnabled|Boolean| Флаг, указывающий, включена ли роль для назначения. Если значение false, роль недоступна для назначения. Только для чтения, если для Builtin задано значение true. |
|resourceScopes|Коллекция String| Список разрешений областей, к которым применяется определение роли. В настоящее время поддерживается только "/". Только для чтения, если для Builtin задано значение true. **НЕ ИСПОЛЬЗУЙТЕ. Это скоро будет рекомендуемым. Присоединение области к назначению роли** | 
|rolePermissions|Коллекция [унифиедролепермиссион](unifiedrolepermission.md)| Список разрешений, включенных в роль. Только для чтения, если для Builtin задано значение true. Обязательный. |
|templateId|String| Настраиваемый идентификатор шаблона, который можно задать, если параметру Builtin присвоено значение false. Этот идентификатор обычно используется, если необходимо, чтобы один идентификатор совпадал для разных каталогов. Только для чтения, если для Builtin задано значение true. |
|version|String| Указывает версию Унифиедроледефинитион. Только для чтения, если для Builtin задано значение true.|

## <a name="relationships"></a>Связи

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