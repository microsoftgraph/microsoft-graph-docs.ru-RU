---
title: ускоренный тип ресурсаWindowsQualityUpdateSettings
description: Сложный тип для хранения параметров ускоренного обновления качества, таких как дата выпуска и дни до принудительной перезагрузки.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 55328cb788ab1994eec2ec7e0f8984577b7b9a3b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805277"
---
# <a name="expeditedwindowsqualityupdatesettings-resource-type"></a>ускоренный тип ресурсаWindowsQualityUpdateSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сложный тип для хранения параметров ускоренного обновления качества, таких как дата выпуска и дни до принудительной перезагрузки.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|qualityUpdateRelease|Строка|Дата выпуска для определения обновления качества.|
|daysUntilForcedReboot|Int32|Количество дней после установки, которые принудительные перезагрузки произойдет.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.expeditedWindowsQualityUpdateSettings",
  "qualityUpdateRelease": "String",
  "daysUntilForcedReboot": 1024
}
```



