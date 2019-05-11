---
title: Тип ресурса iosHomeScreenFolderPage
description: Папка, содержащая приложения с начального экрана
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a8fddc9b33b95418366b68fc348591af0db7b35
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946576"
---
# <a name="ioshomescreenfolderpage-resource-type"></a>Тип ресурса iosHomeScreenFolderPage

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Папка, содержащая приложения с начального экрана

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя страницы папки|
|apps|Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)|Список приложений, которые отображаются на странице в папке. Эта коллекция может включать до 500 элементов.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```




