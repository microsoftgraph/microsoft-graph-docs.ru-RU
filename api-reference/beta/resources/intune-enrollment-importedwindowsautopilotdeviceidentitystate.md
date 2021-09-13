---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Пока не задокументировано.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dde6785fb6a9d7d36e3c123734acbaf6884582ff
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017361"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a>Тип ресурса importedWindowsAutopilotDeviceIdentityState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceImportStatus|[importedWindowsAutopilotDeviceIdentityImportStatus](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|Состояние устройства, сообщаемое службой каталогов устройства (DDS). Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.|
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



