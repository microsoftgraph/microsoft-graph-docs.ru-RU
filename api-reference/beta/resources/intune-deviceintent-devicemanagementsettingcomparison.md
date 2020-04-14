---
title: Тип ресурса Девицеманажементсеттингкомпарисон
description: Объект, представляющий результат сравнения параметров
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c2e807c3f17d2e2cff1a0c807fbe2f0201259049
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453389"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a>Тип ресурса Девицеманажементсеттингкомпарисон

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий результат сравнения параметров

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор параметра|
|displayName|Строка|Отображаемое имя параметра|
|дефинитионид|String|Идентификатор определения параметра для этого экземпляра.|
|куррентвалуежсон|String|Значение параметра шаблона (или) в формате JSON для текущего способа (или)|
|неввалуежсон|String|Представление нового значения параметра шаблона в формате JSON|
|компарисонресулт|[deviceManagementComparisonResult](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|Результат сравнения. Возможные значения: `unknown`, `equal`, `notEqual`, `added`, `removed`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingComparison"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingComparison",
  "id": "String (identifier)",
  "displayName": "String",
  "definitionId": "String",
  "currentValueJson": "String",
  "newValueJson": "String",
  "comparisonResult": "String"
}
```



