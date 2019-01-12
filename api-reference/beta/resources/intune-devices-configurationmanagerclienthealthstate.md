---
title: Тип ресурса configurationManagerClientHealthState
description: Состояние работоспособности клиента диспетчер конфигурации
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4d202b5f672977e8bb1a5fe05ba56937005825ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981744"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a>Тип ресурса configurationManagerClientHealthState

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Состояние работоспособности клиента диспетчер конфигурации
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|state|[configurationManagerClientState](../resources/intune-devices-configurationmanagerclientstate.md)|Текущее состояние клиента диспетчер конфигурации. Возможные значения: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.|
|errorCode|Int32|Код ошибки для неудачных состояния.|
|lastSyncDateTime|DateTimeOffset|Выберите пункт опубликованные даты и времени последней синхронизации с помощью диспетчера управления конфигурацией.|

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





