---
title: тип ресурса iosWebContentFilterSpecificWebsitesAccess
description: Представляет тип параметра фильтра веб-контента iOS, который устанавливает URL-закладки в встроенный браузер iOS. Пример сценария в классе, где преподаватели хотели бы, чтобы учащиеся переориентировали веб-сайты через закладки браузера, настроенные на их устройствах iOS, и не имеют доступа к другим сайтам.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 39fcc4e17ef33fa3f96964f169ec4e2010b0f038
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59095600"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a>тип ресурса iosWebContentFilterSpecificWebsitesAccess

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет тип параметра фильтра веб-контента iOS, который устанавливает URL-закладки в встроенный браузер iOS. Пример сценария в классе, где преподаватели хотели бы, чтобы учащиеся переориентировали веб-сайты через закладки браузера, настроенные на их устройствах iOS, и не имеют доступа к другим сайтам.


Наследует [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|specificWebsitesOnly|[коллекция iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)|URL-закладки, которые будут установлены во встроенный браузер и пользователь, могут получать доступ к веб-сайтам только с помощью закладок. Эта коллекция может содержать не более 500 элементов.|
|websiteList|[коллекция iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)|URL-закладки, которые будут установлены во встроенный браузер и пользователь, могут получать доступ к веб-сайтам только с помощью закладок. Эта коллекция может содержать не более 500 элементов.|

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



