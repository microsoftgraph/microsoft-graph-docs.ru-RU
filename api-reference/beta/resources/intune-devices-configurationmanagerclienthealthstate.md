---
title: Тип ресурса Конфигуратионманажерклиенсеалсстате
description: Состояние работоспособности клиента Configuration Manager
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1c1c707d118b666f52e8a898cd0ad258c5cc8308
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465039"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a>Тип ресурса Конфигуратионманажерклиенсеалсстате

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние работоспособности клиента Configuration Manager

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|state|[configurationManagerClientState](../resources/intune-devices-configurationmanagerclientstate.md)|Текущее состояние клиента Configuration Manager. Возможные значения: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.|
|errorCode|Int32|Код ошибки для состояния сбоя.|
|lastSyncDateTime|DateTimeOffset|Дата и время последней синхронизации с точкой управления Configuration Manager.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientHealthState",
  "state": "String",
  "errorCode": 1024,
  "lastSyncDateTime": "String (timestamp)"
}
```



