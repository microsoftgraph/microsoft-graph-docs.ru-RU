---
title: Тип ресурса windowsKioskMultipleApps
description: Класс, используемый для идентификации конфигурацию разных приложения для базовой конфигурации
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b71b8a57151b08d0297a89dfd815f72d66c2d12a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396030"
---
# <a name="windowskioskmultipleapps-resource-type"></a>Тип ресурса windowsKioskMultipleApps

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, используемый для идентификации конфигурацию разных приложения для базовой конфигурации


Наследуется от [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|apps|[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) коллекции|Это единственный приложений для магазина Windows, чтобы оно было доступно для запуска в меню Пуск. Эта коллекция может содержать не более 128 элементов.|
|showTaskBar|Логический|Этот параметр позволяет администратору задать, отображается ли панель задач.|
|disallowDesktopApps|Логический|Этот параметр показывает, что приложений для настольных систем. По умолчанию установлено значение true.|
|startMenuLayoutXml|Binary|Позволяет администраторам переопределить макет Пуск по умолчанию и не позволяет пользователю изменять его.Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета. XML должен быть в двоичном формате.|

## <a name="relationships"></a>Отношения
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
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```




