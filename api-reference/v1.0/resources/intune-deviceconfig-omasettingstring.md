---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5aaf8b1b50373e8339c8527fba0409fb27631b0512e979e367875f57769b875d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182485"
---
# <a name="omasettingstring-resource-type"></a>Тип ресурса omaSettingString

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение строки параметра OMA.


Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|description|String|Описание. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|omaUri|String|OMA. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|value|String|Значение|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```




