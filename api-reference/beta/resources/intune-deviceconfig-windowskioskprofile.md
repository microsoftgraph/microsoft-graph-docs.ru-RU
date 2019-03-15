---
title: Тип ресурса Виндовскиоскпрофиле
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63f00d8cdb8030a29baccc4a8f29e6c6e562c900
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571951"
---
# <a name="windowskioskprofile-resource-type"></a>Тип ресурса Виндовскиоскпрофиле

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Профилеид|String|Ключ объекта.|
|имя_профиля|Строка|Это понятное имя, используемое для идентификации группы приложений, макета этих приложений в меню "Пуск" и пользователей, которым назначена эта конфигурация киоска.|
|Аппконфигуратион|[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md);|Конфигурация приложения, которая будет использоваться для этой конфигурации киоска.|
|Усераккаунтсконфигуратион|Коллекция [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)|Учетные записи пользователей, которые будут заблокированы для этой конфигурации киоска. Эта коллекция может содержать не более 100 элементов.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskProfile",
  "profileId": "String",
  "profileName": "String",
  "appConfiguration": {
    "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
    "apps": [
      {
        "@odata.type": "microsoft.graph.windowsKioskUWPApp",
        "startLayoutTileSize": "String",
        "name": "String",
        "appType": "String",
        "autoLaunch": true,
        "appUserModelId": "String",
        "appId": "String",
        "containedAppId": "String"
      }
    ],
    "showTaskBar": true,
    "allowAccessToDownloadsFolder": true,
    "disallowDesktopApps": true,
    "startMenuLayoutXml": "binary"
  },
  "userAccountsConfiguration": [
    {
      "@odata.type": "microsoft.graph.windowsKioskVisitor"
    }
  ]
}
```




