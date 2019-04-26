---
title: Тип ресурса Привилежедролеассигнмент
description: 'Представляет назначение привилегированной роли для определенного пользователя. '
localization_priority: Normal
ms.openlocfilehash: 479b6d46dc479134fd0abb46b1a9ffe478611a82
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563426"
---
# <a name="privilegedroleassignment-resource-type"></a>Тип ресурса Привилежедролеассигнмент

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет назначение привилегированной роли для определенного пользователя. 


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Коллекция Привилежедролеассигнмент списка](../api/privilegedroleassignment-list.md) | Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)|Получение коллекции объектов Привилежедролеассигнмент.|
|[Получение privilegedRoleAssignment](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Чтение свойств и связей объекта Привилежедролеассигнмент.|
|[Создание задания](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| Создайте новое назначение путем публикации в коллекции назначений.|
|[Удаление](../api/privilegedroleassignment-delete.md) | Нет |Удаление объекта privilegedRoleAssignment. |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Выполнение назначения ролей как бессрочного.|
|[makeEligible](../api/privilegedroleassignment-makeeligible.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Выполнение назначения ролей как соответствующего требованиям.|
|[my](../api/privilegedroleassignment-my.md)|Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)|Получение привилегированных назначений ролей текущего пользователя.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|expirationDateTime|dateTimeOffset|Дата и время в формате UTC, когда истечет срок действия назначения роли Temporary privileged. Для назначения постоянной роли значение равно null.|
|id|string| Уникальный идентификатор для назначения привилегированной роли. Только для чтения. Он указан в формате "Усерид_ролеид", где userId — это строка GUID для идентификатора пользователя Azure AD, а roleId — строка GUID для идентификатора роли администратора Azure.|
|Повышенный уровень|boolean|**значение true** , если назначение роли активировано. **значение false** , если назначение роли отключено.|
|Ресултмессаже|string|Результирующее сообщение, заданное службой.|
|roleId|string|Идентификатор роли. В формате строки GUID.|
|userId|string|Идентификатор пользователя. В формате строки GUID.|

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|Ролеинфо|[privilegedRole](privilegedrole.md)| Только для чтения. Допускается значение null. Сведения о связанной роли.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
}-->

```json
{
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isElevated": true,
  "resultMessage": "string",
  "roleId": "string",
  "userId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedroleassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
