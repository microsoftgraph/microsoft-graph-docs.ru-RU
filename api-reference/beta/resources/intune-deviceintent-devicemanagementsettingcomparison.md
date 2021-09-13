---
title: тип ресурса deviceManagementSettingComparison
description: Объект, представляющий результат сравнения параметра
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5a2f9dca86529821f24840e209ef10c25014d27b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091407"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a>тип ресурса deviceManagementSettingComparison

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий результат сравнения параметра

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Параметр ID|
|displayName|String|Имя отображения параметра|
|definitionId|String|ID определения параметра для этого экземпляра|
|currentValueJson|String|Представление JSON значения текущего параметра шаблона намерения (или)|
|newValueJson|String|Представление JSON значения нового параметра шаблона|
|comparisonResult|[deviceManagementComparisonResult](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|Настройка результата сравнения. Возможные значения: `unknown`, `equal`, `notEqual`, `added`, `removed`.|

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



