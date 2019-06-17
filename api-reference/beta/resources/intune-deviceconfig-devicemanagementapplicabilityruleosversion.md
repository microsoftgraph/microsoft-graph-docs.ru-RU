---
title: Тип ресурса Девицеманажементаппликабилитирулеосверсион
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c90a026a231998d7cd3ae25ab55ce63c5edb553
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002506"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a>Тип ресурса Девицеманажементаппликабилитирулеосверсион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Миносверсион|String|Минимальная версия ОС для правила применимости.|
|Максосверсион|String|Максимальная версия ОС для правила применимости.|
|name|String|Имя объекта.|
|ruleType|[Девицеманажементаппликабилитирулетипе](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|Тип правила применимости. Возможные значения: `include`, `exclude`.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
  "minOSVersion": "String",
  "maxOSVersion": "String",
  "name": "String",
  "ruleType": "String"
}
```





