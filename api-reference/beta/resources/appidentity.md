---
title: Тип ресурса appIdentity
description: Указывает удостоверение приложения, которое выполнило действие или было изменено. Включает в себя ИД приложения, имя, ИД основного приложения-службы и имя. Этот ресурс вызван API directoryAudit
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: sureshja
ms.openlocfilehash: 2949acd00b3ef494d7fb3999c180631cf8609cc3
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137048"
---
# <a name="appidentity-resource-type"></a>Тип ресурса appIdentity

Пространство имен: microsoft.graph указывает удостоверение приложения, которое выполнило действие или было изменено. Включает в себя ИД приложения, имя, ИД основного приложения-службы и имя. Этот ресурс вызван API [directoryAudit](../api/directoryaudit-get.md)


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|appId|String|Обозначает уникальный идентификатор GUID, представляющий идентификатор приложения в Azure Active Directory.|
|displayName|Строка|Указывает на имя приложения, отображаемую на портале Azure.|
|servicePrincipalId|Строка|Ссылается на уникальный GUID, указывающий ИД основного службы в Azure Active Directory для соответствующего приложения.|
|servicePrincipalName|String|Ссылается на имя основного службы имя приложения в клиенте. |

## <a name="json-representation"></a>Представление в формате JSON

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


