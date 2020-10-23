---
title: Тип ресурса iosNotificationSettings
description: Элемент, описывающий параметры уведомлений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9d3ce8ab638f365793eb7bb6116dc8b6277b9318
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705763"
---
# <a name="iosnotificationsettings-resource-type"></a>Тип ресурса iosNotificationSettings

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|alertType|[иоснотификатионалерттипе](../resources/intune-deviceconfig-iosnotificationalerttype.md)|Определяет тип оповещения для уведомлений, связанных с этим приложением. Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.|
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





