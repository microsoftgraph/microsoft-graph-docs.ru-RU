---
title: Тип ресурса iPv6Range
description: Диапазон IPv6-адресов
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2c30d85a83bb604a5c0ccb6563d6315a183f6497
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971482"
---
# <a name="ipv6range-resource-type"></a>Тип ресурса iPv6Range

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Диапазон IPv6-адресов

Наследуется от ресурса [ipRange](../resources/intune-shared-iprange.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lowerAddress|Строка|Нижний IP-адрес|
|upperAddress|Строка|Верхний IP-адрес|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



