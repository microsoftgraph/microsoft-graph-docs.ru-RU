---
title: Тип ресурса Манажеддевицемоделсандмануфактурерс
description: Модели и производства меатадата для управляемых устройств в учетной записи
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aa241bd17ad8c42074ed74d2d2548777ea8bf3ba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528536"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a>Тип ресурса Манажеддевицемоделсандмануфактурерс

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Модели и производства меатадата для управляемых устройств в учетной записи

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|девицемоделс|Коллекция String|Список моделей для управляемых устройств в учетной записи|
|девицемануфактурерс|Коллекция String|Список производства для управляемых устройств в учетной записи|

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



