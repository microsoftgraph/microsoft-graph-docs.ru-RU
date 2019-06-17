---
title: Тип ресурса Девицеманажементаппликабилитирулеоседитион
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b3baa84aa90af11f18d6c3dcf8ee1aeafecd240
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002520"
---
# <a name="devicemanagementapplicabilityruleosedition-resource-type"></a>Тип ресурса Девицеманажементаппликабилитирулеоседитион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Оседитионтипес|Коллекция [windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md)|Тип выпуска ОС для правила применимости.|
|name|String|Имя объекта.|
|ruleType|[Девицеманажементаппликабилитирулетипе](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|Тип правила применимости. Возможные значения: `include`, `exclude`.|

## <a name="relationships"></a>Отношения
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





