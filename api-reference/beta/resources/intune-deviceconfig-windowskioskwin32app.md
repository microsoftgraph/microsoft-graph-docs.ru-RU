---
title: тип ресурса windowsKioskWin32App
description: KioskModeApp v4 для поддержки приложений Win32
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c940e7c8d2e7c161ed1fbeff5a3ff02039f55205
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59105925"
---
# <a name="windowskioskwin32app-resource-type"></a>тип ресурса windowsKioskWin32App

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

KioskModeApp v4 для поддержки приложений Win32


Наследуется [от windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|Размер плитки приложения для макета старта, унаследованный от [windowsKioskAppBase.](../resources/intune-deviceconfig-windowskioskappbase.md) Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.|
|name|String|Представляет удобное имя приложения, унаследованной от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|Тип приложения, унаследованный от [windowsKioskAppBase.](../resources/intune-deviceconfig-windowskioskappbase.md) Возможные значения: `unknown`, `store`, `desktop`, `aumId`.|
|autoLaunch|Логический|Разрешить автоматическое запуск приложения в режиме киоска с несколькими приложениями, унаследованных от [windowsKioskAppBase.](../resources/intune-deviceconfig-windowskioskappbase.md)|
|classicAppPath|String|Это классическийapppath, используемый приложением v4 Win32 в режиме киоска|
|edgeNoFirstRun|Логический|Edge first run flag for Edge kiosk mode|
|edgeKioskIdleTimeoutMinutes|Int32|Время ожидания в киоске Edge в минутах для режима киоска Edge. Допустимые значения от 0 до 1440|
|edgeKioskType|[windowsEdgeKioskType](../resources/intune-deviceconfig-windowsedgekiosktype.md)|Тип edge-киоска для режима киоска Edge. Возможные значения: `publicBrowsing`, `fullScreen`.|
|edgeKiosk|String|Edge kiosk (URL) для режима киоска Edge|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskWin32App"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskWin32App",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "classicAppPath": "String",
  "edgeNoFirstRun": true,
  "edgeKioskIdleTimeoutMinutes": 1024,
  "edgeKioskType": "String",
  "edgeKiosk": "String"
}
```



