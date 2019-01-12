---
title: Тип ресурса bulkManagedDeviceActionResult
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: adc2b2a6b139ad428cb191fe45a3ca7f4192092a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981779"
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





