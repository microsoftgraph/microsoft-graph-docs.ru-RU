---
title: тип ресурса teamworkActivityTopic
description: Представляет тему уведомления о канале действий.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: aad39f0f28ada3c0b300c5b4fd580a3d2f1b722ed6f6e77741213e87bd569483
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54231448"
---
# <a name="teamworkactivitytopic-resource-type"></a>тип ресурса teamworkActivityTopic

Пространство имен: microsoft.graph

Представляет тему уведомления о канале действий.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|source|teamworkActivityTopicSource|Тип источника. Возможные значения: `entityUrl`, `text`. Для поддерживаемых URL Graph Microsoft, используйте `entityUrl` . Для пользовательского текста используйте `text` .|
|value|String|Значение темы. Если значение свойства **источника** , это должен быть URL Graph `entityUrl` Microsoft. Если вейл `text` есть, это должно быть простое текстовое значение.|
|webUrl|String|При выборе уведомления пользователь щелкает ссылку. **Необязательный,** когда `entityUrl` источник; требуется, **когда источник** `text` .|

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

