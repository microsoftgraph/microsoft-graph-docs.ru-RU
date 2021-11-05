---
title: тип ресурса preAuthorizedApplication
description: Списки предварительно авторизованных клиентских приложений
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 0f28c771f267324a25198edd66ac64ff7bcdaadd
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780543"
---
# <a name="preauthorizedapplication-resource-type"></a>тип ресурса preAuthorizedApplication

Пространство имен: microsoft.graph

Перечислены клиентские приложения, предварительно авторизованные с указанными разрешениями на доступ к API этого приложения. Пользователи не обязаны соглашаться на любое предварительно авторизованного приложения (для указанных разрешений). Однако для любых дополнительных разрешений, не указанных в preAuthorizedApplications (запрашивается, например, с помощью дополнительного согласия), потребуется согласие пользователя.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|appId|String| Уникальный идентификатор приложения. |
|permissionIds|Коллекция String| Уникальный идентификатор [oauth2PermissionScopes,](permissionscope.md) который требуется приложению. |

## <a name="json-representation"></a>Представление в формате JSON
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

