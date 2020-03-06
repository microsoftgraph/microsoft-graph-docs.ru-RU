---
title: Тип ресурса Аппидентити
description: Указывает идентификатор приложения, который выполнил действие или изменился. Включает идентификатор приложения, имя, идентификатор и имя участника службы. Этот ресурс вызывается API Директоряудит
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dc2f6f912eafdacfc05eb11b65140995dfa28cec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532122"
---
# <a name="appidentity-resource-type"></a>Тип ресурса Аппидентити

Пространство имен: microsoft.graph

Указывает идентификатор приложения, который выполнил действие или изменился. Содержит идентификатор приложения, имя и идентификатор и имя участника службы. Этот ресурс используется операцией [Get директоряудит](../api/directoryaudit-get.md) .

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|appId|String|Обозначает уникальный идентификатор GUID, представляющий идентификатор приложения в Azure Active Directory.|
|displayName|Строка|Указывает на имя приложения, отображаемое на портале Azure.|
|сервицепринЦипалид|Строка|Указывает уникальный идентификатор GUID, указывающий идентификатор участника службы в Azure Active Directory для соответствующего приложения.|
|servicePrincipalName|String|— Имя участника-службы — это имя приложения в клиенте. |

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
