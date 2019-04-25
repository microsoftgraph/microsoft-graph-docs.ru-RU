---
title: Тип ресурса Аппидентити
description: Указывает идентификатор приложения, который выполнил действие или изменился. Включает идентификатор приложения, имя, идентификатор и имя участника службы. Этот ресурс вызывается API Директоряудит
localization_priority: Normal
ms.openlocfilehash: ec61782fca0ab4004fab5a55bd4774c0d64afb3a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535678"
---
# <a name="appidentity-resource-type"></a>Тип ресурса Аппидентити
Указывает идентификатор приложения, который выполнил действие или изменился. Включает идентификатор приложения, имя, идентификатор и имя участника службы. Этот ресурс вызывается API [директоряудит](../api/directoryaudit-get.md)


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|appId|String|Обозначает уникальный идентификатор GUID, представляющий идентификатор приложения в Azure Active Directory.|
|displayName|String|Указывает на имя приложения, отображаемое на портале Azure.|
|СервицепринЦипалид|String|Указывает уникальный идентификатор GUID, указывающий идентификатор участника службы в Azure Active Directory для соответствующего приложения.|
|servicePrincipalName|String|— Имя участника-службы — это имя приложения в клиенте. |

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
