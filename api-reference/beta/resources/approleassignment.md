---
title: Тип ресурса appRoleAssignment
description: Используется, чтобы записать, когда пользователю, группе или субъекту-службе присваивается роль приложения в субъекте-службе приложения. Вы можете создавать, читать и удалять роли приложения.
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 14078064fbded840db3850f41d0263bdc0956998
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336048"
---
# <a name="approleassignment-resource-type"></a>Тип ресурса appRoleAssignment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется, чтобы записать, когда пользователю, группе или субъекту-службе присваивается роль приложения для какого-либо приложения.

Назначение роли приложения — это отношение между назначенным субъектом (пользователь, группа или субъект-служба), приложением ресурса (субъект-служба приложения) и ролью приложения, определенной для приложения ресурса.

Если у [роли приложения](approle.md), которая назначена субъекту, есть непустое свойство **value**, оно включается в утверждения **ролей** маркеров, где субъектом может быть назначенный субъект (например, отклики SAML, маркеры идентификаторов, маркеры доступа, определяющие вошедшего пользователя, или маркер доступа, определяющий субъект-службу). Приложения и API используют эти утверждения в логике авторизации.

Пользователю можно назначить роль приложения напрямую. Если роль приложения назначена группе, то эта роль приложения также считается назначенной непосредственным участникам этой группы. Когда пользователю назначается роль приложения для какого-либо приложения, название этого приложения отображается на [портале "Мои приложения](/azure/active-directory/user-help/my-apps-portal-end-user-access) этого пользователя и в [средстве запуска приложений Microsoft 365](https://support.office.com/article/meet-the-office-365-app-launcher-79f12104-6fed-442f-96a0-eb089a3f476a).

Если назначенный субъект является субъектом-службой, то предоставляется [доступ только к приложению](/azure/active-directory/develop/v2-permissions-and-consent#permission-types). Когда пользователь или администратор принимает разрешение с доступом только к приложению, создается назначение роли приложения, в котором назначенный субъект является субъектом-службой для клиентского приложения, а ресурс является субъектом-службой целевого API.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| id | String | Уникальный идентификатор ключа **appRoleAssignment**. Значение NULL не допускается. Только для чтения. |
| creationTimestamp | DateTimeOffset | Время создания назначения роли приложения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`. Только для чтения. |
| principalId | Guid | Уникальный идентификатор (**ИД**) [пользователя](user.md), [группы](group.md) или [субъекта-службы](serviceprincipal.md), которым предоставляется роль приложения. Требуется при создании.  |
| principalType | Строка | Тип назначенного субъекта. Это может быть `User`, `Group` или `ServicePrincipal`. Только для чтения. |
| principalDisplayName | String |Отображаемое имя пользователя, группы или субъекта-службы, которым было предоставлено назначение роли приложения. Только для чтения. Поддерживает `$filter` (`eq` и `startswith`). |
| resourceId | Guid |Уникальный идентификатор (**ИД**) ресурса [субъект-службы](serviceprincipal.md), для которого производится назначение. Требуется при создании. Поддерживает `$filter` (только `eq`). |
| resourceDisplayName | Строка | Отображаемое имя субъекта-службы приложения ресурса, для которого производится назначение.  |
| appRoleId | Guid | Идентификатор (**ИД**) [роли приложения](approle.md), которая назначается субъекту. Эта роль приложения должна предоставляться в свойстве **appRoles** субъекта-службы приложения ресурса (**resourceId**). Если в приложении ресурса не объявлены никакие роли приложения, можно указать ИД роли приложения по умолчанию (`00000000-0000-0000-0000-000000000000`), чтобы указать, что субъект назначен приложению ресурса без каких-либо определенных ролей приложения. Требуется при создании. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRoleAssignment"
}-->

```json
{
  "id": "String",
  "creationTimestamp": "String (timestamp)",
  "principalDisplayName": "String",
  "principalId": "Guid",
  "principalType": "String",
  "resourceDisplayName": "String",
  "resourceId": "Guid",
  "appRoleId": "Guid"
}
```

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
