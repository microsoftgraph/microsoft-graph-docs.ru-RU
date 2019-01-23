---
title: Тип ресурса importedDeviceIdentityResult
description: В результате попытки импорта устройств удостоверений представляет importedDeviceIdentityResult ресурс.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e4a1720fee543b4814430476ebd6c84a0fc33d73
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395806"
---
# <a name="importeddeviceidentityresult-resource-type"></a>Тип ресурса importedDeviceIdentityResult

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В результате попытки импорта устройств удостоверений представляет importedDeviceIdentityResult ресурс.


Наследуется от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список importedDeviceIdentityResults](../api/intune-enrollment-importeddeviceidentityresult-list.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) коллекции|Свойства списка и связей объектов [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .|
|[Получение importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Чтение свойства и связи объекта [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .|
|[Создание importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Создание нового объекта [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .|
|[Удаление importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|Нет|Удаляет [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).|
|[Обновление importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Обновление свойства объекта [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор identity импортированных устройства унаследованные от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|importedDeviceIdentifier|String|Импортированные устройства идентификатор наследуется от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|Тип импорта наследуется идентификатор устройства из [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md). Возможные значения: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Последние изменения даты и времени описания унаследованные от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|createdDateTime|DateTimeOffset|Созданные Дата и время устройства унаследованные от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|lastContactedDateTime|DateTimeOffset|Связаться с даты последнего устройства, унаследованные от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|description|String|Описание устройства унаследованные от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Состояние устройства в Intune наследуется от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md). Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|[Платформа](../resources/intune-enrollment-platform.md)|Платформа устройства. Наследуется от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md). Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|status|Логический|Состояние импортированных устройств удостоверений|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentityResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String",
  "status": true
}
```




