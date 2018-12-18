---
title: Тип ресурса windowsKioskUWPApp
description: Базовый класс для типов приложений
author: tfitzmac
ms.openlocfilehash: 328a91065692a7b315ade5dae86c15d6def320eb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305182"
---
# <a name="windowskioskuwpapp-resource-type"></a>Тип ресурса windowsKioskUWPApp

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Базовый класс для типов приложений

Наследуется от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|Размер плитку приложение для макета Пуск унаследованные от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md). Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.|
|name|Строка|Представляет понятное имя приложения унаследованные от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|
|appUserModelId|String.|Это единственный идентификатор модели приложения пользователя (AUMID), чтобы оно было доступно для использования в полноэкранном режиме запуска|
|appId|String|Это ссылается на Intune приложения, который будет целевой для те же назначения как базовой конфигурации|
|containedAppId|String.|Это ссылается автономные приложения из приложения для Intune|

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
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```





