---
title: Тип ресурса settings
description: Текущие необходимые параметры для пользователя для использования API аналитики.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a7d534aecf6e7ffa427ea175ae06e2b1820435b2
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450816"
---
# <a name="settings-resource-type"></a>Тип ресурса settings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущие обязательные параметры для пользователя с помощью API аналитики.

Чтобы API аналитики возвращал результаты для пользователей, они должны иметь размещенный в облаке почтовый ящик, включенный для Microsoft Graph, имеющий действительную лицензию MyAnalytics и быть участником использования MyAnalytics.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
[Получение параметров](../api/useranalytics-get-settings.md) | [settings](settings.md) | Получение следующих параметров свойства для пользователя.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|хасграфмаилбокс|Boolean|Указывает, размещается ли основной почтовый ящик пользователя в облаке и включено ли для Microsoft Graph.|
|хаслиценсе|Boolean|Указывает, назначена ли лицензия MyAnalytics для пользователя.|
|хасоптедаут|Boolean|Указывает, выбрал ли пользователь из MyAnalytics.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settings",
  "baseType": null
}-->

```json
{
  "hasGraphMailbox": true,
  "hasLicense": true,
  "hasOptedOut": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->