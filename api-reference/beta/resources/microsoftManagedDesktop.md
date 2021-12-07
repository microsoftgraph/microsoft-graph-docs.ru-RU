---
title: тип ресурса microsoftManagedDesktop
description: Представляет конкретные параметры для компьютеры, управляемые Майкрософт, которые позволяют клиентам получать управляемое устройство для облачного компьютера.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 26eadd11fc46ba794249f1d6f1094a000777b5cf
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322786"
---
# <a name="microsoftmanageddesktop-resource-type"></a>тип ресурса microsoftManagedDesktop

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет конкретные параметры для компьютеры, управляемые Майкрософт, которые позволяют клиентам получать управляемое устройство для облачного компьютера.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|profile|Строка|Имя профиля компьютеры, управляемые Майкрософт, с Windows 365 cloud PC.|
|type|[MicrosoftManagedDesktopType](#microsoftmanageddesktoptype-values)|Указывает, позволяет ли политика обеспечения компьютеры, управляемые Майкрософт. Он указывает тип плана, в соответствии с которым устройство управляется, если включена политика провизии. Возможные значения: `notManaged`, `premiumManaged`, `standardManaged`, `starterManaged`, `unknownFutureValue`.|

### <a name="microsoftmanageddesktoptype-values"></a>значения microsoftManagedDesktopType

|Member|Описание|
|:---|:---|
|notManaged|Устройство не управляется компьютеры, управляемые Майкрософт.|
|premiumManaged|Устройство управляется с помощью компьютеры, управляемые Майкрософт премиум-плана.|
|standardManaged|Управление устройством компьютеры, управляемые Майкрософт стандартным планом.|
|starterManaged|Устройство управляется с помощью компьютеры, управляемые Майкрософт стартера.|
|unknownFutureValue|Эволюционирующее значение sentinel. Не следует использовать.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftManagedDesktop"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.microsoftManagedDesktop",
  "type": "String",
  "profile": "String"
}
```
