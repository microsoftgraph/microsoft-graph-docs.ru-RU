---
title: Тип ресурса windowsDeviceAzureADAccount
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 03199726bdc8793516fe84d2c667b5ac89ee67f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979315"
---
# <a name="windowsdeviceazureadaccount-resource-type"></a>Тип ресурса windowsDeviceAzureADAccount

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Н/Д

Наследуется от [windowsDeviceAccount](../resources/intune-devices-windowsdeviceaccount.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|password|Строка|Н/Д Наследуется от ресурса [windowsDeviceAccount](../resources/intune-devices-windowsdeviceaccount.md)|
|userPrincipalName|Строка|Н/Д|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDeviceAzureADAccount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDeviceAzureADAccount",
  "password": "String",
  "userPrincipalName": "String"
}
```





