---
title: Тип ресурса Булкманажеддевицеактионресулт
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b661577af3bcd1282a007555c25eb60b121ce539
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465190"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a>Тип ресурса Булкманажеддевицеактионресулт

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|сукцессфулдевицеидс|Коллекция объектов string|Успешное выполнение устройств|
|фаиледдевицеидс|Коллекция объектов string|Неисправные устройства|
|нотфаунддевицеидс|Коллекция объектов string|Устройства не найдены|
|нотсуппортеддевицеидс|Коллекция объектов string|Неподдерживаемые устройства|

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



