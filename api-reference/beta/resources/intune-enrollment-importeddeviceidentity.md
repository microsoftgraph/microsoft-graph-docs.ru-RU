---
title: тип ресурсов importedDeviceIdentity
description: Ресурс importedDeviceIdentity представляет уникальный идентификатор оборудования устройства, предварительно заданного для предварительной регистрации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6c4b7f6344444a339644b3eef9717b25372962fa1ceb8ba770b80214b97c56c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54185672"
---
# <a name="importeddeviceidentity-resource-type"></a>тип ресурсов importedDeviceIdentity

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс importedDeviceIdentity представляет уникальный идентификатор оборудования устройства, предварительно заданного для предварительной регистрации.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список импортируемыхDeviceIdentities](../api/intune-enrollment-importeddeviceidentity-list.md)|[importedDeviceIdentity collection](../resources/intune-enrollment-importeddeviceidentity.md)|Список свойств и связей [объектов importedDeviceIdentity.](../resources/intune-enrollment-importeddeviceidentity.md)|
|[Получить importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-get.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Чтение свойств и связей [объекта importedDeviceIdentity.](../resources/intune-enrollment-importeddeviceidentity.md)|
|[Создание importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-create.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Создание нового [объекта importedDeviceIdentity.](../resources/intune-enrollment-importeddeviceidentity.md)|
|[Удаление импортируемого объектаDeviceId](../api/intune-enrollment-importeddeviceidentity-delete.md)|Нет|Удаляет [импортируемуюDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).|
|[Обновление importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-update.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Обновление свойств объекта [importedDeviceIdentity.](../resources/intune-enrollment-importeddeviceidentity.md)|
|[Действие importDeviceIdentityList](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection|Пока не задокументировано.|
|[Действие searchExistingIdentities](../api/intune-enrollment-importeddeviceidentity-searchexistingidentities.md)|[importedDeviceIdentity collection](../resources/intune-enrollment-importeddeviceidentity.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор импортируемого удостоверения устройства|
|importedDeviceIdentifier|Строка|Идентификатор импортируемого устройства|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|Тип импортируемого удостоверения устройства. Возможные значения: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Последнее изменение dateTime описания|
|createdDateTime|DateTimeOffset|Время создания даты устройства|
|lastContactedDateTime|DateTimeOffset|Время последней контактной даты устройства|
|description|Строка|Описание устройства|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Состояние устройства в Intune. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|платформа|[платформа](../resources/intune-enrollment-platform.md)|Платформа устройства. Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```




