---
title: тип ресурса windowsKioskMultipleApps
description: Класс, используемый для определения конфигурации приложения MultiMode для конфигурации киоска
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30c7b8d6fe52debe1afa3c7228dc2fc4c2298478
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086423"
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
|showTaskBar|Логическое|Этот параметр позволяет администратору указать, отображается ли панели задач или нет.|
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



