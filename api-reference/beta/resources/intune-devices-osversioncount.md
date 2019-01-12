---
title: Тип ресурса osVersionCount
description: Количество устройств с вредоносных программ для каждой версии операционной системы
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: de841e679ede22492d26f2a1587e775179c45761
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911842"
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





