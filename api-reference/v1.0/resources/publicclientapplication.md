---
title: тип ресурса publicClientApplication
description: Указывает параметры для не веб-приложения или веб-Api. (например, мобильный или другой общедоступный клиент, например установленное приложение, запущенное на настольном устройстве)
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: a5769d2fcbc01114b9a79a6eb3bad21c65566663
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067054"
---
# <a name="publicclientapplication-resource-type"></a>тип ресурса publicClientApplication

Пространство имен: microsoft.graph

Указывает параметры для не-веб-приложения или не-веб-API (например, мобильных или других общедоступных клиентов, таких как установленное приложение, запущенное на настольном устройстве).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|redirectUris|Коллекция String| Указывает URL-адреса, куда отправляются маркеры пользователей для регистрации, или URL-адреса перенаправления, куда отправляются коды авторизации OAuth 2.0 и маркеры доступа. |

## <a name="json-representation"></a>Представление в формате JSON
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

