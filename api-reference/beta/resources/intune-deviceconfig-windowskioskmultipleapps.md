---
title: тип ресурса windowsKioskMultipleApps
description: Класс, используемый для определения конфигурации приложения MultiMode для конфигурации киоска
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 678943374b2db49513ca0739f75cead5565ce99c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58800410"
---
# <a name="windowskioskmultipleapps-resource-type"></a>тип ресурса windowsKioskMultipleApps

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, используемый для определения конфигурации приложения MultiMode для конфигурации киоска


Наследует [от windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|apps|[коллекция windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|Это единственные Windows store Apps, которые будут доступны для запуска из меню . Эта коллекция может содержать не более 128 элементов.|
|showTaskBar|Логический|Этот параметр позволяет администратору указать, отображается ли панели задач или нет.|
|allowAccessToDownloadsFolder|Логический|Этот параметр позволяет получить доступ к папке Downloads в проводнике файлов.|
|disallowDesktopApps|Логический|Этот параметр указывает, что настольные приложения разрешены. По умолчанию значение true.|
|startMenuLayoutXml|Binary|Позволяет администраторам переопределять макет Start по умолчанию и не позволяет пользователю изменять его. Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета. XML должен быть в двоичном формате.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskMultipleApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskMultipleApps",
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
}
```



