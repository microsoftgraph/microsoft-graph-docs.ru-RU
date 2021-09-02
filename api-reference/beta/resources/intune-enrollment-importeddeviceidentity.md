---
title: тип ресурсов importedDeviceIdentity
description: Ресурс importedDeviceIdentity представляет уникальный идентификатор оборудования устройства, предварительно заданного для предварительной регистрации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f1dbcb41d30bec09335316503fbc8f93f6264c34
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803492"
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
|importedDeviceIdentifier|String|Идентификатор импортируемого устройства|
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



