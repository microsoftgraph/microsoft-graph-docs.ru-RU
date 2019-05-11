---
title: Тип ресурса iosNotificationSettings
description: Элемент, описывающий параметры уведомлений.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0503d938860798408fa5eb2af20ac51dc988f8a7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946450"
---
# <a name="iosnotificationsettings-resource-type"></a>Тип ресурса iosNotificationSettings

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Элемент, описывающий параметры уведомлений.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|bundleID|Строка|Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.|
|appName|String|Имя приложения, которое нужно связать со свойством bundleID.|
|publisher|String|Издатель, которого нужно связать со свойством bundleID.|
|enabled|Логический|Указывает, разрешены ли уведомления для этого приложения.|
|showInNotificationCenter|Логический|Указывает, можно ли отображать уведомления в центре уведомлений.|
|showOnLockScreen|Логический|Указывает, можно ли отображать уведомления на экране блокировки.|
|alertType|[Иоснотификатионалерттипе](../resources/intune-deviceconfig-iosnotificationalerttype.md)|Определяет тип оповещения для уведомлений, связанных с этим приложением. Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.|
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




