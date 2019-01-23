---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0a287fcf8be771037a39efd821f5468acf518371
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398326"
---
# <a name="iosnetworkusagerule-resource-type"></a>Тип ресурса iosNetworkUsageRule

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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




