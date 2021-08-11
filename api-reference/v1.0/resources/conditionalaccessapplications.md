---
title: тип ресурса conditionalAccessApplications
description: Представляет приложения и действия пользователей, включенные и исключенные из области политики.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 54bf29579240514b5b5d224e54c6246638c703083df6ab230a44bf66a9c47c69
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54223643"
---
# <a name="conditionalaccessapplications-resource-type"></a>тип ресурса conditionalAccessApplications

Пространство имен: microsoft.graph

Представляет приложения и действия пользователей, включенные в политику и исключенные из нее.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| includeApplications | Коллекция String | Список ID приложений, к который применяется политика, если явно не исключено (в исключенииApplications). Также можно установить `All` . |
| excludeApplications | Коллекция String | Список ID приложений явно исключен из политики. |
| includeUserActions | Коллекция строк | Действия пользователя, которые необходимо включить. Поддерживаемые значения `urn:user:registersecurityinfo` и `urn:user:registerdevice` |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeApplications",
    "excludeApplications",
    "includeUserActions"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessApplications"
}-->

```json
{
  "includeApplications": ["String"],
  "excludeApplications": ["String"],
  "includeUserActions": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessApplications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

