---
title: тип ресурса windowsKioskUWPApp
description: Базовый класс для типа приложений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 98eb1dff676499dc589b0d707a2d81590c2e98e885598d867ef1db3badac3126
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54253049"
---
# <a name="windowskioskuwpapp-resource-type"></a>тип ресурса windowsKioskUWPApp

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый класс для типа приложений


Наследуется [от windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|Размер плитки приложения для макета старта, унаследованный от [windowsKioskAppBase.](../resources/intune-deviceconfig-windowskioskappbase.md) Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.|
|name|String|Представляет удобное имя приложения, унаследованной от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|Тип приложения, унаследованный от [windowsKioskAppBase.](../resources/intune-deviceconfig-windowskioskappbase.md) Возможные значения: `unknown`, `store`, `desktop`, `aumId`.|
|autoLaunch|Логический|Разрешить автоматическое запуск приложения в режиме киоска с несколькими приложениями, унаследованных от [windowsKioskAppBase.](../resources/intune-deviceconfig-windowskioskappbase.md)|
|appUserModelId|Строка|Это единственный ID модели пользователя приложения (AUMID), который будет доступен для запуска использования в режиме киоска|
|appId|String|Это ссылается на приложение Intune, которое будет ориентировано на те же назначения, что и конфигурация киоска|
|containedAppId|Строка|Это ссылается на содержалось приложение из приложения Intune|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskUWPApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```




