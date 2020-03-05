---
title: Тип ресурса Унифиедролеассигнмент
description: Назначение роли — это связь между определением роли и участником в определенной области для предоставления доступа.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c51c3cd7c706cf154db8c1de21c04aaa098c3efb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519619"
---
# <a name="unifiedroleassignment-resource-type"></a>Тип ресурса Унифиедролеассигнмент

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Унифиедролеассигнмент используется для предоставления доступа к ресурсам. Он представляет определение роли, назначенное участнику (обычно пользователю) в определенной области.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение Унифиедролеассигнмент](../api/unifiedroleassignment-get.md) | [унифиедролеассигнмент](unifiedroleassignment.md) | Чтение свойств и связей объекта Унифиедролеассигнмент. |
| [Создание Унифиедролеассигнмент](../api/rbacapplication-post-roleassignments.md) | [унифиедролеассигнмент](unifiedroleassignment.md) | Создание нового Унифиедролеассигнмент путем отправки в коллекцию roleAssignment. |
| [удаление](../api/unifiedroleassignment-delete.md); | Нет | Удаление объекта Унифиедролеассигнмент. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для Унифиедролеассигнмент. Key, не допускающая значение null, только для чтения. |
|principalId|String| ObjectID субъекта, которому предоставляется назначение. |
|ресаурцескопе|String| Область, в которой применяется Унифиедролеассигнмент. Это "/" для всей службы. |
|роледефинитионид|String| Унифиедроледефинитион, для которого предназначено назначение. Только для чтения. |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "principalId": "String",
  "resourceScope": "String",
  "roleDefinitionId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
