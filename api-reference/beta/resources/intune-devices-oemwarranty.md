---
title: тип ресурса oemWarranty
description: Сведения о гарантии OEM для данного устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e64e0018fc185cfb79ecc32990b6c4ad4b02c7d
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292419"
---
# <a name="oemwarranty-resource-type"></a>тип ресурса oemWarranty

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения о гарантии OEM для данного устройства

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|baseWarranties|[коллекция warrantyOffer](../resources/intune-devices-warrantyoffer.md)|Список базовых гарантийных предложений. Эта коллекция может содержать не более 100 элементов.|
|additionalWarranties|[коллекция warrantyOffer](../resources/intune-devices-warrantyoffer.md)|Список дополнительных гарантийных предложений. Эта коллекция может содержать не более 100 элементов.|
|deviceWarrantyUrl|String|URL-адрес страницы гарантии устройства|
|deviceConfigurationUrl|String|URL-адрес страницы конфигурации устройства|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oemWarranty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.oemWarranty",
  "baseWarranties": [
    {
      "@odata.type": "microsoft.graph.warrantyOffer",
      "type": "String",
      "description": "String",
      "startDateTime": "String (timestamp)",
      "endDateTime": "String (timestamp)"
    }
  ],
  "additionalWarranties": [
    {
      "@odata.type": "microsoft.graph.warrantyOffer",
      "type": "String",
      "description": "String",
      "startDateTime": "String (timestamp)",
      "endDateTime": "String (timestamp)"
    }
  ],
  "deviceWarrantyUrl": "String",
  "deviceConfigurationUrl": "String"
}
```




