---
title: Тип ресурса appIdentity
description: Указывает удостоверение приложения, которое выполнило действие или было изменено. Включает id приложения, имя, главный ИД службы и имя. Этот ресурс называется API directoryAudit
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 0d9347ecf3571b89843c6e2b83454d6ae45b5b65405ba66914227a994abc0fb7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54155213"
---
# <a name="appidentity-resource-type"></a>Тип ресурса appIdentity

Пространство имен: microsoft.graph

Указывает удостоверение приложения, которое выполнило действие или было изменено. Включает В себя ID приложения, имя и главный ID службы и имя. Этот ресурс используется операцией [Get directoryAudit.](../api/directoryaudit-get.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|appId|String|Обозначает уникальный идентификатор GUID, представляющий идентификатор приложения в Azure Active Directory.|
|displayName|String|Ссылается на имя приложения, отображаемую на портале Azure.|
|servicePrincipalId|String|Ссылается на уникальный GUID с указанием основного id службы в Azure Active Directory для соответствующего приложения.|
|servicePrincipalName|String|Ссылается на имя главного клиента службы — имя приложения в клиенте. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appIdentity"
}-->

```json
{
  "appId": "String",
  "displayName": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

