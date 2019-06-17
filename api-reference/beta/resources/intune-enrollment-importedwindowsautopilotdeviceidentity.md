---
title: Тип ресурса importedWindowsAutopilotDeviceIdentity
description: Импортированные устройства с Windows AutoPilot
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c5a5058f3930acb8cc1af4acf59254b4fd5ab67c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992572"
---
# <a name="importedwindowsautopilotdeviceidentity-resource-type"></a>Тип ресурса importedWindowsAutopilotDeviceIdentity

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Импортированные устройства с Windows AutoPilot

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список importedWindowsAutopilotDeviceIdentities](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-list.md)|Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|Список свойств и связей между объектами[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).|
|[Получение importedWindowsAutopilotDeviceIdentity](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-get.md)|[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|Чтение свойств и связей между объектами[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).|
|[Создание importedWindowsAutopilotDeviceIdentity](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-create.md)|[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|Создание нового объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).|
|[Удаление importedWindowsAutopilotDeviceIdentity](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-delete.md)|Отсутствует|Удаляет [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).|
|[Обновление importedWindowsAutopilotDeviceIdentity](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-update.md)|[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|Обновляет свойства объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).|
|[действие импорта](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-import.md)|Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID объекта|
|orderIdentifier|String|Номер заказа устройства Windows Autopilot.|
|serialNumber|String|Серийный номер устройства Windows Autopilot.|
|productKey|Строка|Ключ продукта устройства Windows Autopilot.|
|Импортид|String|Идентификатор импорта для устройства автопилота Windows.|
|hardwareIdentifier|Двоичный|Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.|
|state|[importedWindowsAutopilotDeviceIdentityState](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|Текущее состояние импортированного устройства.|
|АссигнедусерпринЦипалнаме|String|Имя участника-пользователя для пользователя, которому будет назначено устройство|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "String (identifier)",
  "orderIdentifier": "String",
  "serialNumber": "String",
  "productKey": "String",
  "importId": "String",
  "hardwareIdentifier": "binary",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "String",
    "deviceRegistrationId": "String",
    "deviceErrorCode": 1024,
    "deviceErrorName": "String"
  },
  "assignedUserPrincipalName": "String"
}
```





