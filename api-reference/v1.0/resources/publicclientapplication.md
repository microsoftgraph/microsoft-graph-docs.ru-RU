---
title: Тип ресурса publicClientApplication
description: Указывает параметры для других веб-приложений и веб-API. (Например, мобильный или другой общедоступный клиент, например установленное приложение, запущенное на настольном устройстве)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: a15f0ea159ab12403186465783200a9e374562bc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137517"
---
# <a name="publicclientapplication-resource-type"></a>Тип ресурса publicClientApplication

Пространство имен: microsoft.graph

Указывает параметры для не веб-приложения или не-веб-API (например, мобильных или других общедоступных клиентов, таких как установленное приложение, запущенное на настольном устройстве).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|redirectUris|Коллекция String| Указывает URL-адреса, в которые отправляются маркеры пользователей для входов, или IS перенаправления, в которые отправляются коды авторизации OAuth 2.0 и маркеры доступа. |

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

