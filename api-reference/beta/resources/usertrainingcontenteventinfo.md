---
title: тип ресурса userTrainingContentEventInfo
description: Представляет сведения о обучающих событиях по назначенной подготовке для пользователей в кампании моделирования атак и обучения.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2771c9924bcd0d3441e404b37f7aa75ec55e9c91
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979772"
---
# <a name="usertrainingcontenteventinfo-resource-type"></a>тип ресурса userTrainingContentEventInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об учебном событии в кампании моделирования атак и обучения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Обозреватель|Строка|Браузер пользователя, откуда было сгенерировано обучающее событие.|
|contentDateTime|DateTimeOffset|Дата и время воспроизведения обучающего контента пользователем.|
|ipAddress|String|IP-адрес пользователя для учебного события.|
|osPlatformDeviceDetails|String|Сведения об операционной системе, платформе и устройстве пользователя для учебного события.|
|potentialScoreImpact|Двойное|Возможное улучшение осанки безопасности клиента после завершения обучения пользователем.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userTrainingContentEventInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userTrainingContentEventInfo",
  "contentDateTime": "String (timestamp)",
  "ipAddress": "String",
  "osPlatformDeviceDetails": "String",
  "browser": "String",
  "potentialScoreImpact": "Double"
}
```

