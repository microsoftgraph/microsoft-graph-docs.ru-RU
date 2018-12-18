---
title: Тип ресурса deviceConfigurationTargetedUserAndDevice
description: Конфликт сводки для набора политик конфигурации устройства.
author: tfitzmac
ms.openlocfilehash: 04b0e31d0f3f099389e4901eb654139d286f4bd8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345243"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a>Тип ресурса deviceConfigurationTargetedUserAndDevice

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Конфликт сводки для набора политик конфигурации устройства.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceId|String|Идентификатор устройства в возврата.|
|deviceName|String|Имя устройства в возврата.|
|userId|String|Идентификатор пользователя в записи.|
|userDisplayName|String|Отображаемое имя пользователя в репозиторий|
|userPrincipalName|Строка|Имя участника-пользователя в репозиторий.|
|lastCheckinDateTime|DateTimeOffset|Время последнего checkin для этой пары пользователя и устройства.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationTargetedUserAndDevice",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "lastCheckinDateTime": "String (timestamp)"
}
```





