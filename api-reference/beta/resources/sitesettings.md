---
title: тип ресурса siteSettings
description: Представляет параметры сайта.
author: k-tsoi
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 210b0f36d0dbbfc9402eec6d0a58a62ae646605a
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64590011"
---
# <a name="sitesettings-resource-type"></a>тип ресурса siteSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры [сайта].

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|LanguageTag|Строка|Тег языка для языка, используемого на этом сайте.|
|timeZone|String|Указывает смещение времени для часового пояса сайта из согласованного универсального времени (UTC).|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteSettings"
}
-->
``` json
{
    "languageTag": "String",
    "timeZone": "String"
}
```

[сайта]: site.md
