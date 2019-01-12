---
title: Тип ресурса iosWebContentFilterSpecificWebsitesAccess
description: Представляет операций ввода-вывода тип параметра фильтра веб-содержимого, который устанавливает закладки URL-адрес в браузере встроенных операций ввода-вывода. Пример сценария находится в классе, где преподавателей, предоставляемых студентов переходить веб-сайтов через браузер закладки, настроенного в своих устройствах iOS и нет доступа на другие сайты.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 3b117aca95c43f36c216d6249221d689ae2da325
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942698"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a>Тип ресурса iosWebContentFilterSpecificWebsitesAccess

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Представляет операций ввода-вывода тип параметра фильтра веб-содержимого, который устанавливает закладки URL-адрес в браузере встроенных операций ввода-вывода. Пример сценария находится в классе, где преподавателей, предоставляемых студентов переходить веб-сайтов через браузер закладки, настроенного в своих устройствах iOS и нет доступа на другие сайты.

Наследуется от [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|specificWebsitesOnly|[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) коллекции|URL-адрес закладки, установленные в встроенных браузера и пользователей можно использовать только для доступа к веб-сайтов через закладки. Эта коллекция может содержать не более 500 элементов.|
|websiteList|[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) коллекции|URL-адрес закладки, установленные в встроенных браузера и пользователей можно использовать только для доступа к веб-сайтов через закладки. Эта коллекция может содержать не более 500 элементов.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
  "specificWebsitesOnly": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ],
  "websiteList": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ]
}
```





