---
title: тип ресурсов importedAppleDeviceIdentity
description: Ресурс importedAppleDeviceIdentity представляет собой импортируемый идентификатор устройства устройства Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f4469d5df6acd7f2ee3ad3e542742d656e72f7a4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863291"
---
# <a name="importedappledeviceidentity-resource-type"></a>тип ресурсов importedAppleDeviceIdentity

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс importedAppleDeviceIdentity представляет собой импортируемый идентификатор устройства устройства Apple.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список импортируемыхAppleDeviceIdentities](../api/intune-enrollment-importedappledeviceidentity-list.md)|[importedAppleDeviceIdentity collection](../resources/intune-enrollment-importedappledeviceidentity.md)|Список свойств и связей импортируемых [объектовAppleDeviceIdentity.](../resources/intune-enrollment-importedappledeviceidentity.md)|
|[Get importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-get.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Чтение свойств и связей объекта [importedAppleDeviceIdentity.](../resources/intune-enrollment-importedappledeviceidentity.md)|
|[Создание объекта importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-create.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Создание нового [объекта importedAppleDeviceIdentity.](../resources/intune-enrollment-importedappledeviceidentity.md)|
|[Удаление импортируемого объектаAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-delete.md)|Нет|Удаляет [импортируемую структуруAppleDeviceId.](../resources/intune-enrollment-importedappledeviceidentity.md)|
|[Обновление импортируемогоAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-update.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Обновление свойств объекта [importedAppleDeviceIdentity.](../resources/intune-enrollment-importedappledeviceidentity.md)|
|[Действие importAppleDeviceIdentityList](../api/intune-enrollment-importedappledeviceidentity-importappledeviceidentitylist.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|serialNumber|String|Серийный номер устройства|
|requestedEnrollmentProfileId|String|Администратор ID профиля регистрации намерен примениться к устройству во время следующей регистрации|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|Профиль времени регистрации был назначен устройству|
|isSupervised|Boolean|Указывает, контролируется ли устройство Apple. Дополнительные сведения можно получить по: https://support.apple.com/en-us/HT202837|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md);|Источник обнаружения устройств Apple. Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|isDeleted|Логический|Указывает, удалено ли устройство из Apple Business Manager|
|createdDateTime|DateTimeOffset|Время создания даты устройства|
|lastContactedDateTime|DateTimeOffset|Время последней контактной даты устройства|
|description|String|Описание устройства|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Состояние устройства в Intune. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|платформа|[платформа](../resources/intune-enrollment-platform.md)|Платформа устройства. Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|

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




