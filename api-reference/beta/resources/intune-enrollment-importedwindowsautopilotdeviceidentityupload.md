---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityUpload
description: Импорт автопилот устройства windows, с помощью отправки.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ea2c2620bf76410aa55d2568c6962fbb96636e3e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394728"
---
# <a name="importedwindowsautopilotdeviceidentityupload-resource-type"></a>Тип ресурса importedWindowsAutopilotDeviceIdentityUpload

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Импорт автопилот устройства windows, с помощью отправки.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список importedWindowsAutopilotDeviceIdentityUploads](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-list.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) коллекции|Свойства списка и связей объектов [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .|
|[Получение importedWindowsAutopilotDeviceIdentityUpload](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-get.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)|Чтение свойства и связи объекта [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .|
|[Создание importedWindowsAutopilotDeviceIdentityUpload](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-create.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)|Создание нового объекта [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .|
|[Удаление importedWindowsAutopilotDeviceIdentityUpload](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-delete.md)|Нет|Удаляет [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).|
|[Обновление importedWindowsAutopilotDeviceIdentityUpload](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-update.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)|Обновление свойства объекта [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .|
|[функция autopilotDeviceStream](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-autopilotdevicestream.md)|String|Создание запроса загрузки с потоком автопилот устройство в нем.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|GUID объекта|
|createdDateTimeUtc|DateTimeOffset|Дата и время при создании сущности.|
|status|[importedWindowsAutopilotDeviceIdentityUploadStatus](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|Отправьте состояние. Возможные значения: `noUpload`, `pending`, `complete`, `error`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|deviceIdentities|Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|Коллекция всех устройств автопилот в рамках этой загрузки.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "String (identifier)",
  "createdDateTimeUtc": "String (timestamp)",
  "status": "String"
}
```




