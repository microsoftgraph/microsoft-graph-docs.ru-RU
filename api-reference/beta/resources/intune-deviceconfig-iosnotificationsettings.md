---
title: Тип ресурса iosNotificationSettings
description: Элемент, описывающий параметры уведомлений.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 07962568b6e44582a3950de4461cb1e57dfb7412
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526327"
---
# <a name="iosnotificationsettings-resource-type"></a>Тип ресурса iosNotificationSettings

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Элемент, описывающий параметры уведомлений.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|bundleID|String|Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.|
|appName|String|Имя приложения, которое нужно связать со свойством bundleID.|
|publisher|String|Издатель, которого нужно связать со свойством bundleID.|
|enabled|Логический|Указывает, разрешены ли уведомления для этого приложения.|
|showInNotificationCenter|Логический|Указывает, можно ли отображать уведомления в центре уведомлений.|
|showOnLockScreen|Логический|Указывает, можно ли отображать уведомления на экране блокировки.|
|alertType|[иоснотификатионалерттипе](../resources/intune-deviceconfig-iosnotificationalerttype.md)|Определяет тип оповещения для уведомлений, связанных с этим приложением. Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.|
|badgesEnabled|Логический|Указывает, разрешены ли эмблемы для этого приложения.|
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



