---
title: тип ресурса answerVariant
description: Вариант ответа можно использовать для изменения определенных свойств ответа поиска в зависимости от страны или платформы.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 99d196273ae772091f236b18d2821288f63eefe9
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339529"
---
# <a name="answervariant-resource-type"></a>тип ресурса answerVariant

Пространство имен: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вариант ответа можно использовать для изменения определенных полей ответа поиска в зависимости от страны или платформы.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|Описание вариантов ответа, показанное на странице результатов поиска.|
|displayName|Строка|Имя варианта ответа, отображаемая в результатах поиска.|
|webUrl|String|Ссылка URL-адрес варианта ответа. Когда пользователи щелкают этот вариант ответа в результатах поиска, они перейдут на этот URL-адрес.|
|LanguageTags|Коллекция строк|Список стран или регионов, которые могут просмотреть этот ответ поиска.|
|платформы|коллекция microsoft.graph.platform|Список устройств и операционных систем, способных просматривать этот вариант ответа. Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.search.answerVariant"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search.answerVariant",
  "displayName": "String",
  "webUrl": "String",
  "description": "String",
  "languageTags": ["String"],
  "platforms": ["String"]
}
```

