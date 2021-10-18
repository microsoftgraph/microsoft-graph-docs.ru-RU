---
title: Тип ресурса windowsDeviceADAccount
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 94ce7543d12bc0fc037b2f54a74315bc13645ace
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60453620"
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



