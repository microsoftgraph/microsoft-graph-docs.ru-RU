---
title: тип ресурса requiredResourceAccess
description: Указывает набор областей разрешений OAuth 2.0 и ролей приложений.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: ea14ac7d38dd44f16c548f5501e17c7e244c5214
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59055873"
---
# <a name="requiredresourceaccess-resource-type"></a>тип ресурса requiredResourceAccess

Пространство имен: microsoft.graph

Указывает набор областей разрешений OAuth 2.0 и ролей приложений в указанном ресурсе, к который приложению требуется доступ. Указанные области разрешений OAuth 2.0 могут запрашиваться клиентские приложения (через коллекцию **requiredResourceAccess)** при вызове приложения-ресурса. Свойство **requiredResourceAccess** объекта [](application.md) приложения — это коллекция **ReqiredResourceAccess.**


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
|resourceAccess|[коллекция resourceAccess](resourceaccess.md)|Список областей разрешений OAuth2.0 и ролей приложений, которые приложение требует от указанного ресурса.|
|resourceAppId|Строка|Уникальный идентификатор для ресурса, к который приложению требуется доступ.  Это должно быть равно **приложению, объявленным** в целевом приложении ресурса.|

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

