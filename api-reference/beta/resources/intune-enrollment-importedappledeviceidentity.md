---
title: Тип ресурса importedAppleDeviceIdentity
description: Ресурс importedAppleDeviceIdentity представляет удостоверение импортированного устройства устройства Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5355f273e2e6535eb877d72efc7e1718fe04e87e
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669065"
---
# <a name="importedappledeviceidentity-resource-type"></a>Тип ресурса importedAppleDeviceIdentity

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс importedAppleDeviceIdentity представляет удостоверение импортированного устройства устройства Apple.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление importedAppleDeviceIdentities](../api/intune-enrollment-importedappledeviceidentity-list.md)|[Коллекция importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Список свойств и связей объектов [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Получение importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-get.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Чтение свойств и связей объекта [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Создание объекта importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-create.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Создайте объект [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Удаление importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-delete.md)|Нет|Удаляет объект [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).|
|[Обновление importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-update.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Обновление свойств объекта [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Действие importAppleDeviceIdentityList](../api/intune-enrollment-importedappledeviceidentity-importappledeviceidentitylist.md)|[Коллекция importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|serialNumber|String|Серийный номер устройства.|
|requestedEnrollmentProfileId|String|Администратор идентификатора профиля регистрации планирует применить к устройству во время следующей регистрации.|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|Профиль регистрации времени, назначенный устройству|
|isSupervised|Boolean|Указывает, защищено ли устройство Apple. Дополнительные сведения см. по адресу: https://support.apple.com/en-us/HT202837|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md);|Источник обнаружения устройств Apple. Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|isDeleted|Логическое|Указывает, удалено ли устройство из Apple Business Manager|
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
  "@odata.type": "microsoft.graph.importedAppleDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "String (identifier)",
  "serialNumber": "String",
  "requestedEnrollmentProfileId": "String",
  "requestedEnrollmentProfileAssignmentDateTime": "String (timestamp)",
  "isSupervised": true,
  "discoverySource": "String",
  "isDeleted": true,
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```




