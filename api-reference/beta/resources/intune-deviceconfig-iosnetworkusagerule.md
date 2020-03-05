---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 99e9f769be7184df600e16544ca19f2c26d56391
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526334"
---
# <a name="iosnetworkusagerule-resource-type"></a>Тип ресурса iosNetworkUsageRule

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|managedApps|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Сведения об управляемых приложениях, к которым применяется это правило. Эта коллекция может содержать не более 500 элементов.|
|cellularDataBlockWhenRoaming|Логический|Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в роуминге.|
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



