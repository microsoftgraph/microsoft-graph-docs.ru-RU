---
title: Тип ресурса Девицеманажементаппликабилитирулеоседитион
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2635332b311c89c7bcea2fab076a905cdf0afa41
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724588"
---
# <a name="devicemanagementapplicabilityruleosedition-resource-type"></a>Тип ресурса Девицеманажементаппликабилитирулеоседитион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|оседитионтипес|Коллекция [windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md)|Тип выпуска ОС для правила применимости.|
|name|String|Имя объекта.|
|ruleType|[deviceManagementApplicabilityRuleType](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|Тип правила применимости. Возможные значения: `include`, `exclude`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
  "osEditionTypes": [
    "String"
  ],
  "name": "String",
  "ruleType": "String"
}
```





