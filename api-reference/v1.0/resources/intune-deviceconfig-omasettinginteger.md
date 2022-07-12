---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 96fe347b217cdd60aab4668dc89731f85448620d
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730016"
---
# <a name="omasettinginteger-resource-type"></a>Тип ресурса omaSettingInteger

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение целого числа параметра OMA.


Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|description|String|Описание. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|omaUri|String|OMA. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|value|Int32|Значение.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```





