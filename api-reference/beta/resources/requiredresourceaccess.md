---
title: Тип ресурса requiredResourceAccess
description: Указывает набор областей разрешений OAuth 2.0 и ролей приложений.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: f9a847e6863353e59602aef3c794bc7d79e40d5e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133723"
---
# <a name="requiredresourceaccess-resource-type"></a>Тип ресурса requiredResourceAccess

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает набор областей разрешений OAuth 2.0 и ролей приложения в указанном ресурсе, к который приложению требуется доступ. Указанные области разрешений OAuth 2.0 могут запрашиваться клиентских приложений (с помощью коллекции **requiredResourceAccess)** при вызове приложения ресурсов. Свойство **requiredResourceAccess** объекта [приложения](application.md) — это коллекция **Re.redResourceAccess.**


## <a name="json-representation"></a>Представление в формате JSON

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
|resourceAccess|[Коллекция ResourceAccess](resourceaccess.md)|Список областей разрешений OAuth2.0 и ролей приложений, необходимых приложению для указанного ресурса.|
|resourceAppId|Строка|Уникальный идентификатор ресурса, к котором приложению требуется доступ.  Он должен быть равен **appId, объявленным** в целевом приложении ресурсов.|

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


