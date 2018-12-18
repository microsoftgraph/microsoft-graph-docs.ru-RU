---
title: Тип ресурса bulkManagedDeviceActionResult
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 0a80a05b1caba7cd5ac1e672c9e39366ca29048c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339517"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a>Тип ресурса bulkManagedDeviceActionResult

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Н/Д
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|successfulDeviceIds|Коллекция String|Успешные устройств|
|failedDeviceIds|Коллекция String|Сбой устройств|
|notFoundDeviceIds|Коллекция String|Не найден устройств|
|notSupportedDeviceIds|Коллекция String|Не поддерживаемые устройства|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bulkManagedDeviceActionResult",
  "successfulDeviceIds": [
    "String"
  ],
  "failedDeviceIds": [
    "String"
  ],
  "notFoundDeviceIds": [
    "String"
  ],
  "notSupportedDeviceIds": [
    "String"
  ]
}
```





