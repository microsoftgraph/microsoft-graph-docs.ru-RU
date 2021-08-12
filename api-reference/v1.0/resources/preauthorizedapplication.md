---
title: тип ресурса preAuthorizedApplication
description: Списки предварительно авторизованных клиентских приложений
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: f59bdd28a23ff92705914ba6361bcce860df4650791c8dcabd22f96753fc0f50
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202149"
---
# <a name="preauthorizedapplication-resource-type"></a>тип ресурса preAuthorizedApplication

Пространство имен: microsoft.graph

Перечислены клиентские приложения, предварительно авторизованные с указанными разрешениями на доступ к API этого приложения. Пользователи не обязаны соглашаться на любое предварительно авторизованного приложения (для указанных разрешений). Однако для любых дополнительных разрешений, не указанных в preAuthorizedApplications (запрашивается, например, с помощью дополнительного согласия), потребуется согласие пользователя.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|appId|String| Уникальный идентификатор приложения. |
|permissionIds|Коллекция String| Уникальный идентификатор [oauth2PermissionScopes,](permissionscope.md) который требуется приложению. |

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

