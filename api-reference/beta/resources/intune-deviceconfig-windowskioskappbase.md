---
title: Тип ресурса Виндовскиоскаппбасе
description: Базовый класс для типа приложений
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d3ba4a27f1107b35264d1671530b5314ea28026c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786448"
---
# <a name="windowskioskappbase-resource-type"></a>Тип ресурса Виндовскиоскаппбасе

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый класс для типа приложений

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|стартлайауттилесизе|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|Размер плитки приложения для начального макета. Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.|
|name|String|Представляет понятное имя приложения.|
|Тип|[виндовскиоскапптипе](../resources/intune-deviceconfig-windowskioskapptype.md)|Тип приложения. Возможные значения: `unknown`, `store`, `desktop`, `aumId`.|
|Автозапуск|Логический|Разрешение автоматического запуска приложения в полноэкранном режиме с поддержкой нескольких приложений|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAppBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAppBase",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true
}
```



