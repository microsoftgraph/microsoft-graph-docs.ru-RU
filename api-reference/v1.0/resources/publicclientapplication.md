---
title: тип ресурса publicClientApplication
description: Указывает параметры для не веб-приложения или веб-Api. (например, мобильный или другой общедоступный клиент, например установленное приложение, запущенное на настольном устройстве)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: b8172eb64c1f54e33f8b5775a9234a7a30a42b641b68dd328c2fef5355fb9688
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54228997"
---
# <a name="publicclientapplication-resource-type"></a>тип ресурса publicClientApplication

Пространство имен: microsoft.graph

Указывает параметры для не-веб-приложения или не-веб-API (например, мобильных или других общедоступных клиентов, таких как установленное приложение, запущенное на настольном устройстве).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|redirectUris|Коллекция String| Указывает URL-адреса, куда отправляются маркеры пользователей для регистрации, или URL-адреса перенаправления, куда отправляются коды авторизации OAuth 2.0 и маркеры доступа. |

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

