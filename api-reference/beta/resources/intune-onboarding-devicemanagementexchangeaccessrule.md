---
title: Тип ресурса Девицеманажементексчанжеакцессруле
description: Правила доступа к устройству в Exchange.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 62d5dac75116278eac6f3d1764dbb8f8865434f4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029654"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a>Тип ресурса Девицеманажементексчанжеакцессруле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Правила доступа к устройству в Exchange.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|девицекласс|[девицеманажементексчанжедевицекласс](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|Класс устройства, на который влияет это правило.|
|accessLevel|[девицеманажементексчанжеакцесслевел](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|Уровень доступа для Exchange, предоставляемый этим правилом. Возможные значения: `none`, `allow`, `block`, `quarantine`.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeAccessRule",
  "deviceClass": {
    "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
    "name": "String",
    "type": "String"
  },
  "accessLevel": "String"
}
```






