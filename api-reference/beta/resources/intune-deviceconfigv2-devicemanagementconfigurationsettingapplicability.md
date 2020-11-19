---
title: Тип ресурса Девицеманажементконфигуратионсеттингаппликабилити
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f94bfffd8dd3149d11e7ada38a4c238f4ce618a4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242192"
---
# <a name="devicemanagementconfigurationsettingapplicability-resource-type"></a>Тип ресурса Девицеманажементконфигуратионсеттингаппликабилити

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|Описание параметра|
|платформа|[девицеманажементконфигуратионплатформс](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Параметр платформы можно применить к. Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.|
|девицемоде|[девицеманажементконфигуратиондевицемоде](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|Режим устройства, к которому можно применять параметры. Возможные значения: `none`, `kiosk`.|
|технологически|[девицеманажементконфигуратионтечнологиес](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Какие технологические каналы можно развернуть с помощью этого параметра. Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingApplicability",
  "description": "String",
  "platform": "String",
  "deviceMode": "String",
  "technologies": "String"
}
```




