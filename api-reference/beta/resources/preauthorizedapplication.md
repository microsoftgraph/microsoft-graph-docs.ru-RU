---
title: Тип ресурса preAuthorizedApplication
description: Список предварительно авторизованных клиентских приложений
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 40fcfc642444be507fbd8e8a85f0052732293cb3
ms.sourcegitcommit: 191b797b178f40fde6419719fcd75461e6869401
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2022
ms.locfileid: "66118538"
---
# <a name="preauthorizedapplication-resource-type"></a>Тип ресурса preAuthorizedApplication

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Выводит список клиентских приложений, предварительно авторизованных с указанными делегированными разрешениями на доступ к API этого приложения. Пользователи не должны давать согласие на какие-либо предварительно авторизованные приложения (для указанных разрешений). Однако все дополнительные разрешения, не перечисленные в preAuthorizedApplications (например, запрашиваемые с помощью добавочного согласия), требуют согласия пользователя.

В некоторых редких случаях идентификатор, указанный в свойстве, может ссылаться на роль [приложения (](approle.md) `appRoles` из свойства субъекта-службы), `appId` указывающую, `permissionIds` что клиентское приложение, определяемое свойством, предварительно авторизовано для этой роли приложения.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|appId|String| Уникальный идентификатор клиентского приложения. |
|permissionIds|Коллекция String| Уникальный идентификатор областей [, которые](permissionscope.md) предоставляет клиентское приложение. |

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
<!--
{
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

