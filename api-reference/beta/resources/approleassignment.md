---
title: Тип ресурса appRoleAssignment
description: Используется для записи, когда пользователь или группа назначается приложения. В этом случае назначения роли приведет к плитки приложения отображается вверх на панели приложения доступа пользователя. Этот объект также могут быть использованы для предоставления другого приложения (смоделирован как основной службы) доступа к приложению ресурсов в определенной роли. Можно создавать, читать, обновление и удаление назначения ролей.
localization_priority: Priority
ms.openlocfilehash: 3276c1f34b91dc628ed00f2ffbc64ffe56899bdf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845474"
---
# <a name="approleassignment-resource-type"></a>Тип ресурса appRoleAssignment

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Используется для записи, когда пользователь или группа назначается приложения. В этом случае назначения роли приведет к плитки приложения отображается вверх на панели приложения доступа пользователя. Этот объект также могут быть использованы для предоставления другого приложения (смоделирован как основной службы) доступа к приложению ресурсов в определенной роли. Можно создавать, читать, обновление и удаление назначения ролей.


## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approleassignment"
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
|creationTimestamp|DateTimeOffset|Время создания разрешений. Тип метки времени представляет сведения даты и времени с использованием формата ISO 8601 и — это всегда в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|Guid|Идентификатор роли, которая была назначена субъекта.  Эта роль должны быть объявлены с приложения ресурсов конечного **Ид_ресурса** в своем свойстве **appRoles** . Где ресурса не объявляет никаких разрешений, должен быть указан идентификатор по умолчанию (нулевое значение GUID). Ключ. Значение null не допускается. |
|principalDisplayName|Строка|Отображаемое имя субъекта, который был предоставлен доступ.|
|principalId|Guid|Уникальный идентификатор (**id**) для участника, которому предоставляется доступ. Требуется при создании.            |
|principalType|Строка|Тип субъекта.  Это может быть «User», «Группы» или «ServicePrincipal».|
|resourceDisplayName|Строка|Отображаемое имя ресурса, к которому назначения.|
|resourceId|Guid|Уникальный идентификатор (**id**) для целевой ресурс, для которого было выполнено назначение (участников-служб).|

## <a name="relationships"></a>Связи
Нет


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение appRoleAssignment](../api/approleassignment-get.md) | [appRoleAssignment](approleassignment.md) |Чтение свойства и связи объекта appRoleAssignment.|
|[обновление](../api/approleassignment-update.md). | [appRoleAssignment](approleassignment.md)   |Обновление объекта appRoleAssignment. |
|[Delete](../api/approleassignment-delete.md) | Нет |Удалите объект appRoleAssignment. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
