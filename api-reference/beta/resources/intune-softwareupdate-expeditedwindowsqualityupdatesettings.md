---
title: ускоренный тип ресурсаWindowsQualityUpdateSettings
description: Сложный тип для хранения параметров ускоренного обновления качества, таких как дата выпуска и дни до принудительной перезагрузки.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8537f7bf9736d5d6e2a7015d3d1f11af7f7be0710698e964465d41311543e3f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54193533"
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




