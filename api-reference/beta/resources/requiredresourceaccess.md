---
title: Тип ресурса Рекуиредресаурцеакцесс
description: Задает набор областей разрешений и ролей приложений для OAuth 2,0.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: a2104052f4c70a988d1154bb08db025e740246fb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938823"
---
# <a name="requiredresourceaccess-resource-type"></a>Тип ресурса Рекуиредресаурцеакцесс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Задает набор областей разрешений OAuth 2,0 и ролей приложения в указанном ресурсе, к которому приложение требует доступ. Указанные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** ) при вызове приложения-ресурса. Свойство **рекуиредресаурцеакцесс** объекта [Application](application.md) представляет собой коллекцию **рекиредресаурцеакцесс**.


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
|resourceAccess|Коллекция [ресаурцеакцесс](resourceaccess.md)|Список областей разрешений OAuth 2.0 и ролей приложений, которые требуются приложению из указанного ресурса.|
|ресаурцеаппид|Строка|Уникальный идентификатор ресурса, доступ к которому требуется приложению.  Он должен быть равен **AppID** , объявленному в целевом приложении ресурсов.|

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
