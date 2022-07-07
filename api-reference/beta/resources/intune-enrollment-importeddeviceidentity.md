---
title: Тип ресурса importedDeviceIdentity
description: Ресурс importedDeviceIdentity представляет собой уникальное аппаратное удостоверение устройства, предварительно подготовленных для настройки перед регистрацией.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 19da44719f1e7f72358350509eec6c52aaeff122
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66667266"
---
# <a name="importeddeviceidentity-resource-type"></a>Тип ресурса importedDeviceIdentity

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс importedDeviceIdentity представляет собой уникальное аппаратное удостоверение устройства, предварительно подготовленных для настройки перед регистрацией.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление importedDeviceIdentities](../api/intune-enrollment-importeddeviceidentity-list.md)|[Коллекция importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Список свойств и связей объектов [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Получение importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-get.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Чтение свойств и связей объекта [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Создание объекта importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-create.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Создайте новый [объект importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Удаление importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-delete.md)|Нет|Удаляет объект [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).|
|[Обновление importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-update.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Обновление свойств объекта [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Действие importDeviceIdentityList](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|[Коллекция importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Пока не задокументировано.|
|[Действие searchExistingIdentities](../api/intune-enrollment-importeddeviceidentity-searchexistingidentities.md)|[Коллекция importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор импортированного удостоверения устройства|
|importedDeviceIdentifier|String|Импортированный идентификатор устройства|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|Тип импортированного удостоверения устройства. Возможные значения: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения описания|
|createdDateTime|DateTimeOffset|Дата создания устройства|
|lastContactedDateTime|DateTimeOffset|Дата последнего контакта устройства|
|description|String|Описание устройства|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Состояние устройства в Intune. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|платформа|[Платформы](../resources/intune-enrollment-platform.md)|Платформа устройства. Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|

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




