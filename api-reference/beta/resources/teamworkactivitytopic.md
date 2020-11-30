---
title: Тип ресурса Теамворкактивититопик
description: Представляет раздел уведомления о канале активности.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a4425053cf41ebfbad139c6d0ea5fc246f0b1391
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377611"
---
# <a name="teamworkactivitytopic-resource-type"></a>Тип ресурса Теамворкактивититопик

Пространство имен: microsoft.graph

Представляет раздел уведомления о канале активности.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|source|теамворкактивититопиксаурце|Тип источника. Возможные значения: `entityUrl`, `text`. Для поддерживаемых URL-адресов Microsoft Graph используйте `entityUrl` . Для настраиваемого текста используйте `text` .|
|value|String|Значение раздела. Если свойство **Source** имеет значение `entityUrl` , это должен быть URL-адрес Microsoft Graph. Если задано `text` значение вауле, это должно быть обычное текстовое значение.|
|webUrl|String|Ссылка, которую пользователь щелкает при выборе уведомления. Необязательный параметр, если **источник** — это `entityUrl` обязательный **параметр** `text` .|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkActivityTopic"
}
-->
```json
{
  "@odata.type": "#microsoft.graph.teamworkActivityTopic",
  "source": "String",
  "value": "String",
  "webUrl": "String"
}
```

