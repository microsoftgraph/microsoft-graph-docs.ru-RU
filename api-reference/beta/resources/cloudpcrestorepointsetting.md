---
title: тип ресурса cloudPcRestorePointSetting
description: Представляет конкретные параметры точеченого восстановления.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 7e49cebd6f3bcb9a6af0ac469608b4c54081a7d8
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339422"
---
# <a name="cloudpcrestorepointsetting-resource-type"></a>тип ресурса cloudPcRestorePointSetting

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры точечного восстановления облачного компьютера.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|frequencyInHours|Int32|Интервал времени в часах для автоматического создания снимков (точек восстановления) облачного КОМПЬЮТЕРА. Возможные значения : `4`, `6`, `12`, и `16``24`. Частота по умолчанию — 12 часов.|
|userRestoreEnabled|Boolean|Если `true`пользователь может использовать снимки для восстановления облачных компьютеров. Если `false`пользователи, не управляющие, не могут использовать снимки для восстановления облачного компьютера.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcRestorePointSetting"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcRestorePointSetting",
  "frequencyInHours": "Integer",
  "userRestoreEnabled": "Boolean"
}
```
