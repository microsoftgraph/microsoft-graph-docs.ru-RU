---
title: тип ресурса windowsKioskUWPApp
description: Базовый класс для типа приложений
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9ef0294701a660219a1c74119cc2af2912a315df
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59105974"
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
|appUserModelId|String|Это единственный ID модели пользователя приложения (AUMID), который будет доступен для запуска использования в режиме киоска|
|appId|String|Это ссылается на приложение Intune, которое будет ориентировано на те же назначения, что и конфигурация киоска|
|containedAppId|String|Это ссылается на содержалось приложение из приложения Intune|

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



