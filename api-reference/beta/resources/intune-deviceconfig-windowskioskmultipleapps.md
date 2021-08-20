---
title: тип ресурса windowsKioskMultipleApps
description: Класс, используемый для определения конфигурации приложения MultiMode для конфигурации киоска
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e7be767a72b68eeff6cf85aa46051222d81d18fe13430d473db96332e1ec57a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54164302"
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




