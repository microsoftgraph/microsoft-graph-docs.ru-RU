---
title: Тип ресурса managedDeviceModelsAndManufacturers
description: Модели и производители meatadata для управляемых устройств в учетной записи
author: tfitzmac
ms.openlocfilehash: 42611b0c14aa583d2871d97b66ce116a0b835268
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352936"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a>Тип ресурса managedDeviceModelsAndManufacturers

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Модели и производители meatadata для управляемых устройств в учетной записи
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceModels|Коллекция String|Список моделей для управляемых устройств в учетной записи|
|deviceManufacturers|Коллекция String|Список производители управляемых устройств в учетной записи|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
  "deviceModels": [
    "String"
  ],
  "deviceManufacturers": [
    "String"
  ]
}
```





