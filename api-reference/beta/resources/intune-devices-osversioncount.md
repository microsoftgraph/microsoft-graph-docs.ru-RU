---
title: Тип ресурса osVersionCount
description: Количество устройств с вредоносных программ для каждой версии операционной системы
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 227e802de7226d653d68997268c9bf4eac4aa259
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864150"
---
# <a name="osversioncount-resource-type"></a>Тип ресурса osVersionCount

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Количество устройств с вредоносных программ для каждой версии операционной системы
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|osVersion|String|Версия операционной системы|
|deviceCount|Int32|Количество устройств с вредоносных программ для версии операционной системы|
|lastUpdateDateTime|DateTimeOffset|Метка времени последнего обновления для счетчик устройства в формате UTC|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```





