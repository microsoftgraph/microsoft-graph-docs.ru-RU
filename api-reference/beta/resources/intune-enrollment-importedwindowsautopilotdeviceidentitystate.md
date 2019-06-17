---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0569bca45ccc7f5ce3a9fbe9953921a1df8f0b9a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992565"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a>Тип ресурса importedWindowsAutopilotDeviceIdentityState

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceImportStatus|[Импортедвиндовсаутопилотдевицеидентитимпортстатус](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|Состояние устройства, сообщаемое службой каталогов устройства (DDS). Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.|
|deviceRegistrationId|String|Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).|
|deviceErrorCode|Int32|Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).|
|deviceErrorName|Строка|Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).|

## <a name="relationships"></a>Отношения
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





