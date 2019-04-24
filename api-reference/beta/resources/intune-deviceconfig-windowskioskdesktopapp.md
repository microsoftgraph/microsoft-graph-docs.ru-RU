---
title: Тип ресурса windowsKioskDesktopApp
description: Базовый класс для типа приложений
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89f309b53e44b0f2843145dd7c0f4d3ffa6d7f98
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453966"
---
# <a name="windowskioskdesktopapp-resource-type"></a>Тип ресурса windowsKioskDesktopApp

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый класс для типа приложений


НаСледуется от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Стартлайауттилесизе|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|Размер плитки приложения для начального макета, унаследованного от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md). Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.|
|name|String|Представляет понятное имя приложения, наСледуемого от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)|
|Тип|[Виндовскиоскапптипе](../resources/intune-deviceconfig-windowskioskapptype.md)|Тип приложения, наСледуемого из [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md). Возможные значения: `unknown`, `store`, `desktop`, `aumId`.|
|Автозапуск|Boolean|Разрешить автоматический запуск приложения в режиме киоска с несколькими приложениями, унаследованном от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)|
|path|String|Определение пути к классическому приложению|
|Десктопаппликатионид|Строка|Определение Десктопаппликатионид приложения|
|Десктопаппликатионлинкпас|Строка|Определение Десктопаппликатионлинкпас приложения|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskDesktopApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```





