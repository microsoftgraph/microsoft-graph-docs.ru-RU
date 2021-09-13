---
title: ускоренный тип ресурсаWindowsQualityUpdateSettings
description: Сложный тип для хранения параметров ускоренного обновления качества, таких как дата выпуска и дни до принудительной перезагрузки.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 127a5ec4e1650cdd4e24787e24757b05732284d3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59029922"
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

## <a name="relationships"></a>Отношения
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



