---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
ms.openlocfilehash: 93cfd1f5eefe6f32fd0b112b24e3cdfba6969434
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078983"
---
# <a name="iosnetworkusagerule-resource-type"></a>Тип ресурса iosNetworkUsageRule

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|managedApps|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Сведения об управляемых приложениях, к которым применяется это правило. Эта коллекция может содержать не более 500 элементов.|
|cellularDataBlockWhenRoaming|Boolean|Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в роуминге.|
|cellularDataBlocked|Boolean|Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в любое время.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNetworkUsageRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNetworkUsageRule",
  "managedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "cellularDataBlockWhenRoaming": true,
  "cellularDataBlocked": true
}
```





