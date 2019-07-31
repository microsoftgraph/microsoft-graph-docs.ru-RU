---
title: Тип ресурса appRoleAssignment
description: Используется для записи при назначении пользователя или группы приложению. В этом случае после назначения роли будет отображаться плитка приложения на панели доступа к приложениям пользователя. Кроме того, с помощью этого объекта можно предоставить другому приложению (моделируемому как субъект-служба) доступ к приложению ресурса в определенной роли. Вы можете создавать, просматривать, обновлять и удалять назначенные роли.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 471927eb3aaf0dc26a3a70b0dffae7e15c812787
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974327"
---
# <a name="approleassignment-resource-type"></a>Тип ресурса appRoleAssignment

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для записи при назначении пользователя или группы приложению. В этом случае после назначения роли будет отображаться плитка приложения на панели доступа к приложениям пользователя. Кроме того, с помощью этого объекта можно предоставить другому приложению (моделируемому как субъект-служба) доступ к приложению ресурса в определенной роли. Вы можете создавать, просматривать, обновлять и удалять назначенные роли.


## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRoleAssignment"
}-->

```json
{
  "creationTimestamp": "String (timestamp)",
  "id": "guid (identifier)",
  "principalDisplayName": "string",
  "principalId": "guid",
  "principalType": "string",
  "resourceDisplayName": "string",
  "resourceId": "guid"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|creationTimestamp|DateTimeOffset|Время создания контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: . Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|GUID|Идентификатор роли, назначенный субъекту.  Эта роль должна быть объявлена в целевом приложении-ресурсе **resourceId** в свойстве **appRoles**. Если в ресурсе не объявлены разрешения, необходимо указать идентификатор по умолчанию (нулевой GUID). Ключ. Значение null не допускается. |
|principalDisplayName|String|Отображаемое имя субъекта, которому был предоставлен доступ.|
|principalId|GUID|Уникальный идентификатор (**id**) для субъекта, которому предоставлен доступ. Требуется при создании.            |
|principalType|String|Тип субъекта.  Это может "Пользователь", "Группа" или "Субъект-служба".|
|resourceDisplayName|String|Отображаемое имя ресурса, для которого было выполнено назначение.|
|resourceId|GUID|Уникальный идентификатор (**id**) для целевого ресурса (субъект-служба), для которого было выполнено назначение.|

## <a name="relationships"></a>Связи
Нет


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта appRoleAssignment](../api/approleassignment-get.md) | [appRoleAssignment](approleassignment.md) |Чтение свойств и связей объекта appRoleAssignment.|
|[Обновление](../api/approleassignment-update.md) | [appRoleAssignment](approleassignment.md)   |Обновление объекта appRoleAssignment. |
|[Удаление](../api/approleassignment-delete.md) | Нет |Удаление объекта appRoleAssignment. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
