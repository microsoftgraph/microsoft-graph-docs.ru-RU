---
title: Тип ресурса iosHomeScreenFolderPage
description: Папка, содержащая приложения с начального экрана
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e28d9e63214e4dc6564423876e7bd041e51bcc60
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992341"
---
# <a name="ioshomescreenfolderpage-resource-type"></a>Тип ресурса iosHomeScreenFolderPage

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Папка, содержащая приложения с начального экрана

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя страницы папки|
|apps|Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)|Список приложений, которые отображаются на странице в папке. Эта коллекция может включать до 500 элементов.|

## <a name="relationships"></a>Отношения
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





