---
title: тип ресурса requiredResourceAccess
description: Указывает набор областей разрешений OAuth 2.0 и ролей приложений.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 374d88cd9cc0166c003618af4382aafe498eaf87
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60452834"
---
# <a name="requiredresourceaccess-resource-type"></a>тип ресурса requiredResourceAccess

Пространство имен: microsoft.graph

Указывает набор областей разрешений OAuth 2.0 и ролей приложений в указанном ресурсе, к который приложению требуется доступ. Приложение [](application.md) может запрашивать указанные области разрешений OAuth 2.0 или роли приложений через свойство **requiredResourceAccess,** которое является коллекцией объектов [requiredResourceAccess.](requiredresourceaccess.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|resourceAccess|[коллекция resourceAccess](resourceaccess.md)|Список областей разрешений OAuth2.0 и ролей приложений, которые приложение требует от указанного ресурса.|
|resourceAppId|String|Уникальный идентификатор для ресурса, к который приложению требуется доступ. Это должно быть равно **приложению, объявленным** в целевом приложении ресурса.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [
    {
      "@odata.type": "microsoft.graph.resourceAccess"
    }
  ],
  "resourceAppId": "String"
}

```


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

