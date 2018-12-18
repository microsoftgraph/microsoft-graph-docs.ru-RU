---
title: Тип ресурса windowsKioskMultipleApps
description: Класс, используемый для идентификации конфигурацию разных приложения для базовой конфигурации
author: tfitzmac
ms.openlocfilehash: 30591e15d29b06ffb807c8b435d0e3c8a6a1b0fa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330144"
---
# <a name="windowskioskmultipleapps-resource-type"></a>Тип ресурса windowsKioskMultipleApps

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Класс, используемый для идентификации конфигурацию разных приложения для базовой конфигурации

Наследуется от [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|apps|[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) коллекции|Это единственный приложений для магазина Windows, чтобы оно было доступно для запуска в меню Пуск.|
|showTaskBar|Boolean.|Этот параметр позволяет администратору задать, отображается ли панель задач.|
|disallowDesktopApps|Boolean.|Этот параметр показывает, что приложений для настольных систем. По умолчанию установлено значение true.|
|startMenuLayoutXml|Binary|Позволяет администраторам переопределить макет Пуск по умолчанию и не позволяет пользователю изменять его.Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета. XML должен быть в двоичном формате.|

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





