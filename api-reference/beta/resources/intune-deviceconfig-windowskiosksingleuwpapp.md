---
title: Тип ресурса Виндовскиосксинглеувпапп
description: Класс, используемый для определения сведений о приложении UWP для конфигурации киоска
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 05042fe7d0285c593dfd325aa9b186808e85bc2f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529023"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a>Тип ресурса Виндовскиосксинглеувпапп

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, используемый для определения сведений о приложении UWP для конфигурации киоска


Наследуется от [виндовскиоскаппконфигуратион](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|увпапп|[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md);|Это единственный идентификатор пользовательской модели приложения (AUMID), который будет доступен для запуска в режиме киоска|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskSingleUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskSingleUWPApp",
  "uwpApp": {
    "@odata.type": "microsoft.graph.windowsKioskUWPApp",
    "startLayoutTileSize": "String",
    "name": "String",
    "appType": "String",
    "autoLaunch": true,
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```



