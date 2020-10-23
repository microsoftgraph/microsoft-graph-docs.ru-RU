---
title: Тип ресурса windowsKioskMultipleApps
description: Класс, используемый для определения конфигурации приложения с многорежимным режимом для конфигурации киоска
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a3aa6b6b20359ec6d8423b48b53c323f237c42e7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729513"
---
# <a name="windowskioskmultipleapps-resource-type"></a>Тип ресурса windowsKioskMultipleApps

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, используемый для определения конфигурации приложения с многорежимным режимом для конфигурации киоска


Наследуется от [виндовскиоскаппконфигуратион](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|apps|Коллекция [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)|Это единственные приложения Магазина Windows, которые будут доступны для запуска из меню "Пуск". Эта коллекция может содержать не более 128 элементов.|
|шовтаскбар|Логический|Этот параметр позволяет администратору указать, отображается ли панель задач.|
|алловакцесстодовнлоадсфолдер|Логический|Этот параметр разрешает доступ к папке "загрузки" в проводнике.|
|дисалловдесктопаппс|Логический|Этот параметр указывает, что классические приложения разрешены. Значение по умолчанию — true.|
|startMenuLayoutXml|Binary|Позволяет администраторам переопределять макет запуска по умолчанию и запрещает пользователю изменять его. Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета. XML должен быть в двоичном формате.|

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





