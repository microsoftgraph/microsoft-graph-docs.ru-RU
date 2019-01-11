---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 73995f6b8f5e376de53ec88772dc3713cc179f3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838607"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a>Тип ресурса windowsInformationProtectionIPRangeCollection

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Коллекция диапазонов IP-адресов Windows Information Protection
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя|
|ranges|Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)|Коллекция диапазонов IP-адресов|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```





