---
title: тип ресурса managedDeviceModelsAndManufacturers
description: Модели и производство meatadata для управляемых устройств в учетной записи
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1b560cb95766d3216b566d33cfe00db2689c6efd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137800"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a>тип ресурса managedDeviceModelsAndManufacturers

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Модели и производство meatadata для управляемых устройств в учетной записи

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceModels|Коллекция объектов string|Список моделей управляемых устройств в учетной записи|
|deviceManufacturers|Коллекция объектов string|Список производителей управляемых устройств в учетной записи|

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



