---
title: тип ресурса teamworkActivityTopic
description: Представляет тему уведомления о канале действий.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: abf2372aca7d58061f609c97521795f328af89f6
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51474018"
---
# <a name="teamworkactivitytopic-resource-type"></a>тип ресурса teamworkActivityTopic

Пространство имен: microsoft.graph

Представляет тему уведомления о канале действий.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|source|teamworkActivityTopicSource|Тип источника. Возможные значения: `entityUrl`, `text`. Для поддерживаемых URL-адресов Microsoft Graph используйте `entityUrl` . Для пользовательского текста используйте `text` .|
|value|String|Значение темы. Если значение свойства **источника** , это должен `entityUrl` быть URL-адрес Microsoft Graph. Если вейл `text` есть, это должно быть простое текстовое значение.|
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

