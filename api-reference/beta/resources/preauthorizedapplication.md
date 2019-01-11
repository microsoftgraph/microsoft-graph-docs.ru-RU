---
title: Тип ресурса preAuthorizedApplication
description: Представляет приложение и запрошенные разрешения для явного согласия пользователя. Требуется администраторам предоставляются разрешения для приложения. preAuthorizedApplications пользователя согласие на запрошенные разрешения не требуются. Разрешения, перечисленные в preAuthorizedApplications не требуют согласия пользователя. Тем не менее любые дополнительные запрошенные разрешения, не указанные в preAuthorizedApplications требуется согласия пользователя.
localization_priority: Normal
ms.openlocfilehash: fa26b8046b81db70300b8ff40abcbd2b84f3f0c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832797"
---
# <a name="preauthorizedapplication-resource-type"></a>Тип ресурса preAuthorizedApplication

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет приложение и запрошенные разрешения для явного согласия пользователя. Требуется администраторам предоставляются разрешения для приложения. preAuthorizedApplications пользователя согласие на запрошенные разрешения не требуются. Разрешения, перечисленные в preAuthorizedApplications не требуют согласия пользователя. Тем не менее любые дополнительные запрошенные разрешения, не указанные в preAuthorizedApplications требуется согласия пользователя.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
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
