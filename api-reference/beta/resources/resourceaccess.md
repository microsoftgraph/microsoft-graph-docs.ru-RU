---
title: Тип ресурса resourceAccess
description: Задает область разрешений для OAuth 2.0 или роль приложения, требующие приложения. Свойство **resourceAccess** типа requiredResourceAccess — это коллекция **ResourceAccess**.
localization_priority: Normal
ms.openlocfilehash: f5389915897c3aab8b8277a45b54042bc861b290
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862337"
---
# <a name="resourceaccess-resource-type"></a>Тип ресурса resourceAccess

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Задает область разрешений для OAuth 2.0 или роль приложения, требующие приложения. Свойство **resourceAccess** типа [requiredResourceAccess](requiredresourceaccess.md) — это коллекция **ResourceAccess**.


## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Guid|Уникальный идентификатор для одного из экземпляров [oAuth2Permission](oauth2permission.md) или [роли приложения](approle.md) , которые предоставляет доступ к приложению ресурсов.|
|type|Строка|Указывает, будет ли свойство **id** ссылается на [oAuth2Permission](oauth2permission.md) или [роли приложения](approle.md). Возможные значения: «область» или «роли».|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
