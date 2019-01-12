---
title: Тип ресурса windowsKioskDesktopApp
description: Базовый класс для типов приложений
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a9b808bfd67e1b14e0b11fe84da48b77b4d965ba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947332"
---
# <a name="windowskioskdesktopapp-resource-type"></a>Тип ресурса windowsKioskDesktopApp

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Базовый класс для типов приложений

Наследуется от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|Размер плитку приложение для макета Пуск унаследованные от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md). Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.|
|name|String|Представляет понятное имя приложения унаследованные от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|
|path|String|Определение пути классического приложения|
|desktopApplicationId|String|Определение DesktopApplicationID приложения|
|desktopApplicationLinkPath|String|Определение DesktopApplicationLinkPath приложения|

## <a name="relationships"></a>Связи
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
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```





