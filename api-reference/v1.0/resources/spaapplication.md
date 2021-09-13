---
title: тип ресурса spaApplication
description: Указывает параметры для одно-страницного приложения.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 6511dfc95523098c96448bf2f39dbedc313217cc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136348"
---
# <a name="spaapplication-resource-type"></a>тип ресурса spaApplication

Пространство имен: microsoft.graph

Указывает параметры для одно-страницного приложения.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| redirectUris | Коллекция String | Указывает URL-адреса, куда отправляются маркеры пользователей для регистрации, или URL-адреса перенаправления, куда отправляются коды авторизации OAuth 2.0 и маркеры доступа. |

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.spaApplication"
}-->

```json
{
  "redirectUris": ["String"]
}
```
