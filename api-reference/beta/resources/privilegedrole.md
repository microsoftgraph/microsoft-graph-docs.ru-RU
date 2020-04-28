---
title: Тип ресурса Привилежедроле
description: 'Представляет роль администратора Azure AD, например: **глобальному администратору, администратору выставления счетов, администратору служб, администратору пользователей, администратору паролей**и т. д.'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 51114eea797d27886f48c664d06d0b88d4a35a2d
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217913"
---
# <a name="privilegedrole-resource-type"></a>Тип ресурса Привилежедроле

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет роль администратора Azure AD, например: **глобальному администратору, администратору выставления счетов, администратору служб, администратору пользователей, администратору паролей**и т. д.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список объектов Привилежедроле](../api/privilegedrole-list.md) | Коллекция [privilegedRole](privilegedrole.md)|Получение коллекции Привилежедроле.|
|[Получение privilegedRole](../api/privilegedrole-get.md) | [privilegedRole](privilegedrole.md) |Чтение свойств и связей объекта Привилежедроле.|
|[Перечисление заданий](../api/privilegedrole-list-assignments.md) |Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)| Получение коллекции объектов назначений для этой роли.|
|[selfActivate](../api/privilegedrole-selfactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Активируйте назначенную роль.|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Деактивация назначенной роли.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|строка|Уникальный идентификатор для роли администратора. Это строка GUID, имеющая то же значение, что и идентификатор шаблона роли из Azure AD для заданной роли. Только для чтения.|
|name|string|Имя роли.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
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
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
  "suppressions": []
}
-->
