---
title: Тип ресурса windowsKioskMultipleApps
description: Класс, используемый для определения конфигурации приложения с многоРежимным режимом для конфигурации киоска
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c657300cf3ca00482b85b7983f28b4df3135c97d
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30570845"
---
# <a name="windowskioskmultipleapps-resource-type"></a>Тип ресурса windowsKioskMultipleApps

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, используемый для определения конфигурации приложения с многоРежимным режимом для конфигурации киоска


НаСледуется от [виндовскиоскаппконфигуратион](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|apps|Коллекция [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)|Это единственные приложения Магазина Windows, которые будут доступны для запуска из меню "Пуск". Эта коллекция может содержать не более 128 элементов.|
|Шовтаскбар|Boolean|Этот параметр позволяет администратору указать, отображается ли панель задач.|
|Алловакцесстодовнлоадсфолдер|Boolean|Этот параметр разрешает доступ к папке "загрузки" в проводнике.|
|Дисалловдесктопаппс|Boolean|Этот параметр указывает, что классические приложения разрешены. Значение по умолчанию — true.|
|startMenuLayoutXml|Binary|Позволяет администраторам переопределять макет запуска по умолчанию и запрещает пользователю изменять его.Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета. XML должен быть в двоичном формате.|

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




