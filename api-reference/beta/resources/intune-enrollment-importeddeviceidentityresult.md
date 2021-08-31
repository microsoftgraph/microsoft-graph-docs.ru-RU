---
title: тип ресурсов importedDeviceIdentityResult
description: Ресурс importedDeviceIdentityResult представляет результат попытки импорта удостоверения устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ce45e2556fde4632227afe16ff270de2ec68c471
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785733"
---
# <a name="importeddeviceidentityresult-resource-type"></a>тип ресурсов importedDeviceIdentityResult

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс importedDeviceIdentityResult представляет результат попытки импорта удостоверения устройства.


Наследуется [от importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список импортируемыхDeviceIdentityResults](../api/intune-enrollment-importeddeviceidentityresult-list.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection|Список свойств и связей [импортируемых объектовDeviceIdentityResult.](../resources/intune-enrollment-importeddeviceidentityresult.md)|
|[Получить importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Чтение свойств и связей [импортируемого объектаDeviceIdentityResult.](../resources/intune-enrollment-importeddeviceidentityresult.md)|
|[Создание importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Создание нового [объекта importedDeviceIdentityResult.](../resources/intune-enrollment-importeddeviceidentityresult.md)|
|[Удаление importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|Нет|Удаление [импортируемогоDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).|
|[Обновление importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Обновление свойств импортируемого [объектаDeviceIdentityResult.](../resources/intune-enrollment-importeddeviceidentityresult.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор импортируемого удостоверения устройства, унаследованный от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|importedDeviceIdentifier|Строка|Импортируемый идентификатор устройства, унаследованный от [импортируемогоDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|Тип импортируемого удостоверения устройства, унаследованный от [импортируемогоDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md). Возможные значения: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Последнее изменение dateTime описания, унаследованной от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|createdDateTime|DateTimeOffset|Время создания даты устройства, унаследованной от [импортируемогоDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|lastContactedDateTime|DateTimeOffset|Время последней контактируемой даты устройства, унаследованной от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|description|Строка|Описание устройства, унаследованной от [импортируемогоDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Состояние устройства в Intune Наследуется от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md). Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|платформа|[платформа](../resources/intune-enrollment-platform.md)|Платформа устройства. Наследуется [от importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md). Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|status|Логический|Состояние удостоверения импортируемого устройства|

## <a name="relationships"></a>Связи
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



