---
title: Тип ресурса publicClientApplication
description: Задает параметры для веб-API без веб-приложения или веб-API. (например, мобильный или другой общедоступный клиент, например, установленное приложение, запущенное на настольном устройстве)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: fc920fe09a891248310e8acebafb4f2da4d36723
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533939"
---
# <a name="publicclientapplication-resource-type"></a>Тип ресурса publicClientApplication

Пространство имен: microsoft.graph

Задает параметры для невеб-приложения или API, не являющихся веб-приложениями (например, мобильных или других общедоступных клиентов, таких как установленное приложение, запущенное на настольном устройстве).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|редиректурис|Коллекция String| Задает URL-адреса, по которым маркеры пользователей отправляются для входа, или URI перенаправления, для которых отправляются коды авторизации OAuth 2,0 и маркеры доступа. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publicClientApplication"
}-->

```json
{
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
