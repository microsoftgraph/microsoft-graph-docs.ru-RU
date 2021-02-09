---
title: Тип ресурса expeditedWindowsQualityUpdateSettings
description: Сложный тип для хранения параметров автоматического обновления качества, таких как дата и дни выпуска до принудительной перезагрузки.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 700b86d15737c75cbf10679ea6e944726d667431
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160610"
---
# <a name="expeditedwindowsqualityupdatesettings-resource-type"></a>Тип ресурса expeditedWindowsQualityUpdateSettings

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сложный тип для хранения параметров автоматического обновления качества, таких как дата выпуска и дни до принудительной перезагрузки.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|qualityUpdateRelease|String|Дата выпуска для определения обновления качества.|
|daysUntilForcedReboot|Int32|Количество дней после установки, в течение чего произойдет принудительный перезагруза.|

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




