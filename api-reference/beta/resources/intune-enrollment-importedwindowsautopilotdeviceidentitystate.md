---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8b9496c593cb714d830aa143918adcf87bed09c8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49197907"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a>Тип ресурса importedWindowsAutopilotDeviceIdentityState

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceImportStatus|[импортедвиндовсаутопилотдевицеидентитимпортстатус](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|Состояние устройства, сообщаемое службой каталогов устройства (DDS). Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.|
|deviceRegistrationId|Строка|Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).|
|deviceErrorCode|Int32|Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).|
|deviceErrorName|Строка|Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
  "deviceImportStatus": "String",
  "deviceRegistrationId": "String",
  "deviceErrorCode": 1024,
  "deviceErrorName": "String"
}
```




