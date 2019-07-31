---
title: Тип ресурса Манажеддевицемоделсандмануфактурерс
description: Модели и производства меатадата для управляемых устройств в учетной записи
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7cfedad0fce093d8fc3358afcf622ac8beb58d6b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999776"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a>Тип ресурса Манажеддевицемоделсандмануфактурерс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Модели и производства меатадата для управляемых устройств в учетной записи

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Девицемоделс|Коллекция строк|Список моделей для управляемых устройств в учетной записи|
|Девицемануфактурерс|Коллекция строк|Список производства для управляемых устройств в учетной записи|

## <a name="relationships"></a>Отношения
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





