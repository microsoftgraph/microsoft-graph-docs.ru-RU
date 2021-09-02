---
title: Тип ресурса iosHomeScreenFolderPage
description: Страница для папки, содержащей приложения и веб-клипы на домашнем экране.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3b72ce408f748b9c79163c5993c4c13ddf0b1615
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786987"
---
# <a name="ioshomescreenfolderpage-resource-type"></a>Тип ресурса iosHomeScreenFolderPage

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Страница для папки, содержащей приложения и веб-клипы на домашнем экране.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя страницы папки|
|apps|Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)|Список приложений и веб-клипов, которые будут отображаться на странице в папке. Эта коллекция может содержать не более 500 элементов.|

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
      "bundleID": "String",
      "isWebClip": true
    }
  ]
}
```



