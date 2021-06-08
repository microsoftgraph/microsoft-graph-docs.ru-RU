---
title: Тип ресурса omaSettingBoolean
description: Логическое определение параметров OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3674e9d7efb438f5afb18e6fdb5b46a261086236
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760246"
---
# <a name="omasettingboolean-resource-type"></a>Тип ресурса omaSettingBoolean

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Логическое определение параметров OMA.


Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|description|String|Описание. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|omaUri|String|OMA. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|value|Boolean|Значение|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```




