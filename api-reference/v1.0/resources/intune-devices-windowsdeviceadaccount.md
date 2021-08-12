---
title: Тип ресурса windowsDeviceADAccount
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 422f8aa2099c04fa46ca0543fec1c6b11d2c660ce04ed8002d0eb308c5ddedbd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243415"
---
# <a name="windowsdeviceadaccount-resource-type"></a>Тип ресурса windowsDeviceADAccount

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д


Наследуется от ресурса [windowsDeviceAccount](../resources/intune-devices-windowsdeviceaccount.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|password|Строка|Н/Д. Наследуется от [windowsDeviceAccount](../resources/intune-devices-windowsdeviceaccount.md)|
|domainName|String|Н/Д|
|userName|String|Н/Д|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDeviceADAccount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDeviceADAccount",
  "password": "String",
  "domainName": "String",
  "userName": "String"
}
```




