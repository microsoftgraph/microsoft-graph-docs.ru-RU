---
title: тип ресурса requiredResourceAccess
description: Указывает набор областей разрешений OAuth 2.0 и ролей приложений.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 24d4e48fb6a15fabb61552d1ee2f2d884f276e6a862706b290fb97c1a2a78096
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54184496"
---
# <a name="requiredresourceaccess-resource-type"></a>тип ресурса requiredResourceAccess

Пространство имен: microsoft.graph

Указывает набор областей разрешений OAuth 2.0 и ролей приложений в указанном ресурсе, к который приложению требуется доступ. Указанные области разрешений OAuth 2.0 могут запрашиваться клиентские приложения (через коллекцию **requiredResourceAccess)** при вызове приложения-ресурса. Свойство **requiredResourceAccess** объекта [](application.md) приложения — это коллекция **ReqiredResourceAccess.**


## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [{"@odata.type": "microsoft.graph.resourceAccess"}],
  "resourceAppId": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|resourceAccess|[коллекция resourceAccess](resourceaccess.md)|Список областей разрешений OAuth2.0 и ролей приложений, которые приложение требует от указанного ресурса.|
|resourceAppId|String|Уникальный идентификатор для ресурса, к который приложению требуется доступ.  Это должно быть равно **приложению, объявленным** в целевом приложении ресурса.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

