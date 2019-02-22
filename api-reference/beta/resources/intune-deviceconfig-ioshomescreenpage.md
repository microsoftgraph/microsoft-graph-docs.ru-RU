---
title: Тип ресурса iosHomeScreenPage
description: Страница, содержащая приложения и папки с начального экрана
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c958570caa81cff7add1e174cbb678fc68cecd87
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149541"
---
# <a name="ioshomescreenpage-resource-type"></a>Тип ресурса iosHomeScreenPage

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Страница, содержащая приложения и папки с начального экрана

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя страницы|
|icons|Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)|Список приложений и папок, отображающихся на странице. Эта коллекция может включать до 500 элементов.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "String",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "String",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "String",
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ]
}
```




