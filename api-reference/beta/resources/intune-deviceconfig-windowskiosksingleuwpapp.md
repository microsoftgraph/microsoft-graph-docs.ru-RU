---
title: Тип ресурса Виндовскиосксинглеувпапп
description: Класс, используемый для определения сведений о приложении UWP для конфигурации киоска
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 804dd2f34416eecb956b322a0f178daaf39b2418
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142044"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a>Тип ресурса Виндовскиосксинглеувпапп

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, используемый для определения сведений о приложении UWP для конфигурации киоска


НаСледуется от [виндовскиоскаппконфигуратион](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Увпапп|[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md);|Это единственный идентификатор пользовательской модели приложения (AUMID), который будет доступен для запуска в режиме киоска|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskSingleUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskSingleUWPApp",
  "uwpApp": {
    "@odata.type": "microsoft.graph.windowsKioskUWPApp",
    "startLayoutTileSize": "String",
    "name": "String",
    "appType": "String",
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```




