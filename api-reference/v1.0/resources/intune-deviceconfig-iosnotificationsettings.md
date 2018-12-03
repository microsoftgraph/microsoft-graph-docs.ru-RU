---
title: Тип ресурса iosNotificationSettings
description: Элемент, описывающий параметры уведомлений.
ms.openlocfilehash: 40f23c228bf10cfb7f273efbe343c1ff773ac280
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027504"
---
# <a name="iosnotificationsettings-resource-type"></a>Тип ресурса iosNotificationSettings

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Элемент, описывающий параметры уведомлений.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|bundleID|String|Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.|
|appName|String|Имя приложения, которое нужно связать со свойством bundleID.|
|publisher|String|Издатель, которого нужно связать со свойством bundleID.|
|enabled|Boolean|Указывает, разрешены ли уведомления для этого приложения.|
|showInNotificationCenter|Boolean|Указывает, можно ли отображать уведомления в центре уведомлений.|
|showOnLockScreen|Boolean|Указывает, можно ли отображать уведомления на экране блокировки.|
|alertType|[iosNotificationAlertType](../resources/intune-deviceconfig-iosnotificationalerttype.md)|Определяет тип оповещения для уведомлений, связанных с этим приложением. Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.|
|badgesEnabled|Boolean|Указывает, разрешены ли эмблемы для этого приложения.|
|soundsEnabled|Boolean|Указывает, разрешены ли звуковые сигналы для этого приложения.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true
}
```



