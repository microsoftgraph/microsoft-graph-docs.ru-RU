---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0e8e2cfe0626d56aeb945bd2bd3446c8f19ba039
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60453002"
---
# <a name="iosnetworkusagerule-resource-type"></a>Тип ресурса iosNetworkUsageRule

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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



