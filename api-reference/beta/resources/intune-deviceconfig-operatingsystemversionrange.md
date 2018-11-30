---
title: Тип ресурса operatingSystemVersionRange
description: Диапазон версии операционной системы.
ms.openlocfilehash: af140bf2a5d889b66d45460465e47c466bb2160b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076867"
---
# <a name="operatingsystemversionrange-resource-type"></a>Тип ресурса operatingSystemVersionRange

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Диапазон версии операционной системы.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|описание|String|Описание этого диапазона (например действительно 1702 сборок)|
|lowestVersion|String|Низший включительно версия, которая содержит этот диапазон.|
|highestVersion|String|Наибольший включительно версию, которая содержит этот диапазон.|

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





