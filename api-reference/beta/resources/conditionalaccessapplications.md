---
title: Тип ресурса conditionalAccessApplications
description: Представляет приложения и действия пользователей, включенные в область политики и исключаемые из нее.
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b7c92b9eab03adb284fdde95794c45fc4f7be19d
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668078"
---
# <a name="conditionalaccessapplications-resource-type"></a>Тип ресурса conditionalAccessApplications

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет приложения и действия пользователей, включенные в политику условного доступа и исключенные из нее.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| includeApplications | Коллекция String | Допустимые значения: <li> Список идентификаторов клиентов (**appId**), к которым применяется политика, если явно не исключен (в **excludeApplications**) <li> `All` <li> `Office365`- Список приложений, включенных в `Office365`список, см. в разделе целевых приложений условного доступа[: Office 365](/azure/active-directory/conditional-access/concept-conditional-access-cloud-apps) |
| excludeApplications | Коллекция String | Допустимые значения: <li> Список идентификаторов клиентов (**appId**), явно исключенных из политики.<li> `Office365`- Список приложений, включенных в `Office365`список, см. в разделе целевых приложений условного доступа[: Office 365](/azure/active-directory/conditional-access/concept-conditional-access-cloud-apps) |
| includeUserActions | Коллекция объектов string | Включаемые действия пользователя. Поддерживаются следующие значения:`urn:user:registersecurityinfo``urn:user:registerdevice` |
| includeAuthenticationContextClassReferences | Коллекция строк | Ссылки на класс контекста проверки подлинности включают в себя. Поддерживаемые значения выполняются `c1` через `c25`. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление JSON

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

