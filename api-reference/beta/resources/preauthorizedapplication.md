---
title: Тип ресурса preAuthorizedApplication
description: Представляет приложение и запрошенные разрешения для явного согласия пользователя. Требуется администраторам предоставляются разрешения для приложения. preAuthorizedApplications пользователя согласие на запрошенные разрешения не требуются. Разрешения, перечисленные в preAuthorizedApplications не требуют согласия пользователя. Тем не менее любые дополнительные запрошенные разрешения, не указанные в preAuthorizedApplications требуется согласия пользователя.
ms.openlocfilehash: d299aefcac541407e0e42d0b0933e903afa3e84d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082428"
---
# <a name="preauthorizedapplication-resource-type"></a>Тип ресурса preAuthorizedApplication

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет приложение и запрошенные разрешения для явного согласия пользователя. Требуется администраторам предоставляются разрешения для приложения. preAuthorizedApplications пользователя согласие на запрошенные разрешения не требуются. Разрешения, перечисленные в preAuthorizedApplications не требуют согласия пользователя. Тем не менее любые дополнительные запрошенные разрешения, не указанные в preAuthorizedApplications требуется согласия пользователя.

## <a name="properties"></a>Свойства

| Свойство | Тип | Description |
|:---------------|:--------|:----------|
|appId|String| Уникальный идентификатор для приложения. |
|permissionIds|Коллекция String| Уникальный идентификатор для [publishedPermissionScope](permissionscope.md) или [роли приложения](approle.md) приложения требуется. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "permissionIds": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->