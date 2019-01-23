---
title: Тип ресурса windowsKioskUWPApp
description: Базовый класс для типов приложений
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7ba5367721890f02af3b348ad469b15024de4800
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392684"
---
# <a name="windowskioskuwpapp-resource-type"></a>Тип ресурса windowsKioskUWPApp

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый класс для типов приложений


Наследуется от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|Размер плитку приложение для макета Пуск унаследованные от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md). Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.|
|name|String|Представляет понятное имя приложения унаследованные от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|
|Тип|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|Тип приложения унаследованные от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md). Возможные значения: `unknown`, `store`, `desktop`, `aumId`.|
|appUserModelId|String|Это единственный идентификатор модели приложения пользователя (AUMID), чтобы оно было доступно для использования в полноэкранном режиме запуска|
|appId|String|Это ссылается на Intune приложения, который будет целевой для те же назначения как базовой конфигурации|
|containedAppId|String|Это ссылается автономные приложения из приложения для Intune|

## <a name="relationships"></a>Отношения
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
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```




