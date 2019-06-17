---
title: Тип ресурса Девицеманажементсеттингкомпарисон
description: Объект, представляющий результат сравнения параметров
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f68ffd08945662fc291fb5489de67967d3cd1cbf
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002002"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a>Тип ресурса Девицеманажементсеттингкомпарисон

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий результат сравнения параметров

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор параметра|
|displayName|Строка|Отображаемое имя параметра|
|Дефинитионид|String|Идентификатор определения параметра для этого экземпляра.|
|Куррентвалуежсон|String|Значение параметра шаблона (или) в формате JSON для текущего способа (или)|
|Неввалуежсон|String|Представление нового значения параметра шаблона в формате JSON|
|Компарисонресулт|[Девицеманажементкомпарисонресулт](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|Результат сравнения. Возможные значения: `unknown`, `equal`, `notEqual`, `added`, `removed`.|

## <a name="relationships"></a>Отношения
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





