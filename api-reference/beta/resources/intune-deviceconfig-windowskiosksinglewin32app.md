---
title: тип ресурса windowsKioskSingleWin32App
description: Класс, используемый для определения конфигурации одного приложения для конфигурации киоска win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1e5d46ff9fb5289cbb0fb7d015f91a97604df552
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58790397"
---
# <a name="windowskiosksinglewin32app-resource-type"></a>тип ресурса windowsKioskSingleWin32App

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, используемый для определения конфигурации одного приложения для конфигурации киоска win32


Наследует [от windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|win32App|[windowsKioskWin32App](../resources/intune-deviceconfig-windowskioskwin32app.md)|Это приложение win32, которое будет доступно для запуска использования в режиме киоска|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskSingleWin32App"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskSingleWin32App",
  "win32App": {
    "@odata.type": "microsoft.graph.windowsKioskWin32App",
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
}
```



