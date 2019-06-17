---
title: Тип ресурса Конфигуратионманажерклиенсеалсстате
description: Состояние работоспособности клиента Configuration Manager
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 618282f2a061ec8327ff93d1af441e088523260b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983241"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a>Тип ресурса Конфигуратионманажерклиенсеалсстате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние работоспособности клиента Configuration Manager

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|state|[configurationManagerClientState](../resources/intune-devices-configurationmanagerclientstate.md)|Текущее состояние клиента Configuration Manager. Возможные значения: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.|
|errorCode|Int32|Код ошибки для состояния сбоя.|
|lastSyncDateTime|DateTimeOffset|Дата и время последней синхронизации с точкой управления Configuration Manager.|

## <a name="relationships"></a>Отношения
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





