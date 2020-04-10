---
title: Тип ресурса Унифиедролеассигнментмултипле
description: Назначение роли — это связь между определением роли и участником в определенной области для предоставления доступа.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 20e0d7a213ea6e46db9cf9774c46bda0070ecd27
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218032"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a>Тип ресурса Унифиедролеассигнментмултипле

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Унифиедролеассигнментмултипле используется для предоставления доступа к ресурсам. Он представляет определение роли, назначенное массиву субъектов (как правило, пользователем), на массивах областей. Примером такого поставщика RBAC является Microsoft Intune. В Microsoft Intune можно создать назначение роли с несколькими участниками и несколькими областями.

Указание **директорископеидс** или **аппскопеидс** является обязательным.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-get.md) | [унифиедролеассигнментмултипле](unifiedroleassignmentmultiple.md) | Чтение свойств и связей объекта Унифиедролеассигнментмултипле. |
| [Создание unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-post.md) | [унифиедролеассигнментмултипле](unifiedroleassignmentmultiple.md) | Создание нового Унифиедролеассигнментмултипле путем отправки в коллекцию roleAssignment. |
| [Обновление unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-update.md) | [унифиедролеассигнментмултипле](unifiedroleassignmentmultiple.md) | Обновление существующего объекта Унифиедролеассигнментмултипле. |
| [Удаление unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-delete.md) | Нет | Удаление объекта Унифиедролеассигнментмултипле. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| id | String | Уникальный идентификатор для Унифиедролеассигнментмултипле. Key, не допускающая значение null, только для чтения. |
| displayName | Строка | Имя назначения роли. |
| description | String | Описание назначения роли. |
| роледефинитионид | Строка | Идентификатор Унифиедроледефинитион, для которого предназначено назначение. Только для чтения. |
| roleDefinition | [унифиедроледефинитион](unifiedroledefinition.md) |Свойство, определяющее roleDefinition, для которого предназначено назначение. Предоставляется таким образом, чтобы абоненты могли получить определение роли `$expand` одновременно с получением назначения роли. |
| принЦипалидс | Коллекция String | ObjectID субъектов, которым предоставляется назначение. |
| субъектов| Коллекция [directoryObject](directoryobject.md) | Коллекция, доступная только для чтения, ссылающаяся на назначенные субъекты. Предоставляется таким образом, чтобы абоненты могли получать участников с `$expand` помощью одновременно с получением назначения роли. Только для чтения. |
| директорископеидс | Коллекция String | Идентификаторы объектов каталога, представляющие области назначения. Области назначения определяют набор ресурсов, доступ к которым получают участники. Области каталогов — это общие области, которые хранятся в каталоге, который понимается несколькими приложениями. Области приложений — это области, которые определены и поняты только для этого приложения. |
| директорископес | Коллекция [directoryObject](directoryobject.md) | Коллекция, доступная только для чтения, ссылающаяся на объекты каталога, которые являются областью назначения. Предоставляется таким образом, чтобы абоненты могли получать объекты каталога `$expand` с использованием одновременно с получением назначения роли. Только для чтения. |
| аппскопеидс | Коллекция String | Идентификаторы определенных областей приложений, когда области назначения относятся к приложениям. Области назначения определяют набор ресурсов, доступ к которым предоставлен субъекту. Области каталогов — это общие области, которые хранятся в каталоге, который понимается несколькими приложениями. Используйте "/" для области действия на уровне клиента. Области приложений — это области, которые определены и поняты только для этого приложения. |
| аппскопес | Коллекция [аппскопе](appscope.md) |Коллекция, доступная только для чтения, с подробными сведениями о конкретных областях приложения, когда области назначения относятся только к приложениям. Сущность вложения. |

## <a name="relationships"></a>Отношения

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "roleDefinitionId": "String",
  "roleDefinition": {"@odata.type": "microsoft.graph.unifiedRoleDefinition"},
  "principalIds": ["string"],
  "principals": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "directoryScopeIds": ["string"],
  "directoryScopes": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "appScopeIds": ["string"],
  "appScopes": [{"@odata.type": "microsoft.graph.appScope"}],
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignmentMultiple resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->