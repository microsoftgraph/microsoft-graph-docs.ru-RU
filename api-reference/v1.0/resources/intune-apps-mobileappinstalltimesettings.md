---
title: Тип ресурса Мобилеаппинсталлтимесеттингс
description: Содержит свойства, используемые для определения времени предоставления приложения устройствам и для установки приложения на устройствах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 77e12b4d22920cccb51aa9a2980f9fc84f95403e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48096063"
---
# <a name="mobileappinstalltimesettings-resource-type"></a>Тип ресурса Мобилеаппинсталлтимесеттингс

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для определения времени предоставления приложения устройствам и для установки приложения на устройствах.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|уселокалтиме|Boolean|Следует ли использовать время локального устройства или время в формате UTC при определении доступных и крайних сроков.|
|startDateTime|DateTimeOffset|Время, когда приложение должно быть доступно для установки.|
|деадлинедатетиме|DateTimeOffset|Время установки приложения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallTimeSettings",
  "useLocalTime": true,
  "startDateTime": "String (timestamp)",
  "deadlineDateTime": "String (timestamp)"
}
```





