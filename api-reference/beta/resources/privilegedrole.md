---
title: Тип ресурса Привилежедроле
description: 'Представляет роль администратора Azure AD, например: глобальному **администратору, администратору выставленИя счетов, администратору служб, администратору пользователей, администратору паролей**и т. д.'
localization_priority: Normal
ms.openlocfilehash: 131999f52a583400b018e98d2319118f69ca87e8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563430"
---
# <a name="privilegedrole-resource-type"></a>Тип ресурса Привилежедроле

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет роль администратора Azure AD, например: глобальному **администратору, администратору выставленИя счетов, администратору служб, администратору пользователей, администратору паролей**и т. д.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список объектов Привилежедроле](../api/privilegedrole-list.md) | Коллекция [privilegedRole](privilegedrole.md)|Получение коллекции Привилежедроле.|
|[Получение privilegedRole](../api/privilegedrole-get.md) | [privilegedRole](privilegedrole.md) |Чтение свойств и связей объекта Привилежедроле.|
|[Перечисление заданий](../api/privilegedrole-list-assignments.md) |Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)| Получение коллекции объектов назначений для этой роли.|
|[selfActivate](../api/privilegedrole-selfactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Активируйте назначенную роль.|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|ДеАктивация назначенной роли.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|строка|Уникальный идентификатор для роли администратора. Это строка GUID, имеющая то же значение, что и идентификатор шаблона роли из Azure AD для заданной роли. Только для чтения.|
|name|string|Имя роли.|

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|assignments|Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)| Назначения для этой роли. Только для чтения. Допускается значение null.|
|settings|[privilegedRoleSettings](privilegedrolesettings.md)| Параметры для этой роли. Только для чтения. Допускается значение null.|
|summary|[privilegedRoleSummary](privilegedrolesummary.md)| Сводные данные для этой роли. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRole"
}-->

```json
{
  "id": "string (identifier)",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
