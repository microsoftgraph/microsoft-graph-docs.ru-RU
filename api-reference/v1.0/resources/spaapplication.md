---
title: тип ресурса spaApplication
description: Указывает параметры для одно-страницного приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 25f907aa8c7e5b47960bb3a482b9745c488d16a9
ms.sourcegitcommit: be09568fa07ab793cd1db500f537ca94ca9e5b4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836988"
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
