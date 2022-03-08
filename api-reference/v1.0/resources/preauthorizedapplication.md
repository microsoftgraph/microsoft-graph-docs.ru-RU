---
title: тип ресурса preAuthorizedApplication
description: Списки предварительно авторизованных клиентских приложений
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 79a186ebc899f54f4915183a0afd6eaab8eca9fe
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334361"
---
# <a name="preauthorizedapplication-resource-type"></a>тип ресурса preAuthorizedApplication

Пространство имен: microsoft.graph

Перечислены клиентские приложения, предварительно авторизованные с указанными разрешениями на доступ к API этого приложения. Пользователи не обязаны соглашаться на любое предварительно авторизованного приложения (для указанных разрешений). Однако для любых дополнительных разрешений, не указанных в preAuthorizedApplications (запрашивается, например, с помощью дополнительного согласия), потребуется согласие пользователя.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|appId|String| Уникальный идентификатор приложения. |
|delegatedPermissionIds|Коллекция объектов string| Уникальный идентификатор [oauth2PermissionScopes](permissionscope.md) , который требуется приложению. |

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
  "delegatedPermissionIds": ["String"]
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

