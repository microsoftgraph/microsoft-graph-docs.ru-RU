---
title: тип ресурса teamworkActivityTopic
description: Представляет тему уведомления о канале действий.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0438234e1e771fc822cf2f5d5742ffa14cf72e36
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123904"
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

