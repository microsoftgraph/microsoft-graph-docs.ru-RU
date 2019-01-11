---
title: Тип ресурса operatingSystemVersionRange
description: Диапазон версии операционной системы.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 56df6b53dc29247d3f718ad185152069a071a0f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875805"
---
# <a name="operatingsystemversionrange-resource-type"></a>Тип ресурса operatingSystemVersionRange

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Диапазон версии операционной системы.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|описание|Строка|Описание этого диапазона (например действительно 1702 сборок)|
|lowestVersion|Строка|Низший включительно версия, которая содержит этот диапазон.|
|highestVersion|Строка|Наибольший включительно версию, которая содержит этот диапазон.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```





