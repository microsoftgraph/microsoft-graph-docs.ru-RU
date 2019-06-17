---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bb5df5f786eefc1b7b7159b1643f9d3d46d8300
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958706"
---
# <a name="omasetting-resource-type"></a>Тип ресурса omaSetting

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение параметра OMA.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя.|
|description|String|Описание.|
|omaUri|String|OMA.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```





