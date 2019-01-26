---
title: Тип ресурса publicClient
description: Задает параметры для без веб-приложения или веб-Api. (например, Mobile или других общедоступных клиентом, например установленные приложения, запущенного на устройстве настольных систем)
localization_priority: Normal
ms.openlocfilehash: 866e27b4ea3e1386b7cc69f967635d38641f121c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571844"
---
# <a name="publicclient-resource-type"></a>Тип ресурса publicClient

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Задает параметры для без веб-приложения или веб-Api. (например, Mobile или других общедоступных клиентом, например установленные приложения, запущенного на устройстве настольных систем)

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|redirectUris|Коллекция String| Указывает URL-адресов, которые будут отправлены маркеры пользователя для входа в или отправки коды авторизации коды URI, OAuth 2.0 и маркеры доступа для перенаправления. |

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
  "suppressions": [
    "Error: /api-reference/beta/resources/publicclient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
