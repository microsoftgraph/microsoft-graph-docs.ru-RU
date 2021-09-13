---
title: Тип ресурса iosHomeScreenFolderPage
description: Страница для папки, содержащей приложения и веб-клипы на домашнем экране.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8c2ab79ac9fd460638d4530240362ffe9536a542
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111189"
---
# <a name="ioshomescreenfolderpage-resource-type"></a>Тип ресурса iosHomeScreenFolderPage

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Страница для папки, содержащей приложения и веб-клипы на домашнем экране.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя страницы папки|
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



