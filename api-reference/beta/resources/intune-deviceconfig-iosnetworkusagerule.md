---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 80d051c8b22023e101a73437bb1d6d3adec2c0be
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803015"
---
# <a name="iosnetworkusagerule-resource-type"></a>Тип ресурса iosNetworkUsageRule

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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



