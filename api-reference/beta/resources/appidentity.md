---
title: Тип ресурса appIdentity
description: Указывает удостоверение приложения, которое выполнило действие или было изменено. Включает id приложения, имя, главный ИД службы и имя. Этот ресурс называется API directoryAudit
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: sureshja
ms.openlocfilehash: 1a2314d76b1b51e0c1a1845f306b5d9a7e78caea
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057889"
---
# <a name="appidentity-resource-type"></a>Тип ресурса appIdentity

Пространство имен: microsoft.graph указывает удостоверение приложения, которое выполнило действие или было изменено. Включает id приложения, имя, главный ИД службы и имя. Этот ресурс называется API [directoryAudit](../api/directoryaudit-get.md)


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


