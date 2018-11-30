---
title: Тип ресурса publicClient
description: Задает параметры для без веб-приложения или веб-Api. (например, Mobile или других общедоступных клиентом, например установленные приложения, запущенного на устройстве настольных систем)
ms.openlocfilehash: ba921fecb554a8749a9020508c538c68a7ff342e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075450"
---
# <a name="publicclient-resource-type"></a>Тип ресурса publicClient

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Задает параметры для без веб-приложения или веб-Api. (например, Mobile или других общедоступных клиентом, например установленные приложения, запущенного на устройстве настольных систем)

## <a name="properties"></a>Свойства

| Свойство | Тип | Description |
|:---------------|:--------|:----------|
|redirectUris|Коллекция String| Указывает URL-адресов, которые будут отправлены маркеры пользователя для входа в или отправки коды авторизации коды URI, OAuth 2.0 и маркеры доступа для перенаправления. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.installedClient"
}-->

```json
{
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->