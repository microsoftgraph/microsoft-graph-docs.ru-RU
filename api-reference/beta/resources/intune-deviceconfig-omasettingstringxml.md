---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d8dbc23845f62c5f2a70af9051efa732b3d3d8ad
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807373"
---
# <a name="omasettingstringxml-resource-type"></a>Тип ресурса omaSettingStringXml

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение строки параметра OMA в формате XML.


Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|description|String|Описание. Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|omaUri|Строка|OMA. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|fileName|String|Имя файла, связанное со свойством Value (XML).|
|value|Двоичный|Значение (массив байтов в кодировке UTF8).|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```





