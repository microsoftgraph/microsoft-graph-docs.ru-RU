---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b14b632e03160e9b56de1ad2ba0c2e32a1b74179
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728979"
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





