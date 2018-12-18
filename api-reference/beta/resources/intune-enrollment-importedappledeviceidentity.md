---
title: Тип ресурса importedAppleDeviceIdentity
description: Ресурс importedAppleDeviceIdentity представляет идентификатор импортированных устройства устройства Apple.
author: tfitzmac
ms.openlocfilehash: 966e384b63026def366ba19ea634d635d77d9083
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317593"
---
# <a name="importedappledeviceidentity-resource-type"></a>Тип ресурса importedAppleDeviceIdentity

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Ресурс importedAppleDeviceIdentity представляет идентификатор импортированных устройства устройства Apple.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список importedAppleDeviceIdentities](../api/intune-enrollment-importedappledeviceidentity-list.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) коллекции|Свойства списка и связей объектов [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Получение importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-get.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Чтение свойства и связи объекта [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Создание importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-create.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Создание нового объекта [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Удаление importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-delete.md)|Нет|Удаляет [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).|
|[Обновление importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-update.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Обновление свойства объекта [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Действие importAppleDeviceIdentityList](../api/intune-enrollment-importedappledeviceidentity-importappledeviceidentitylist.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) коллекции|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|serialNumber|Строка|Серийный номер устройства|
|requestedEnrollmentProfileId|String.|Admin идентификатор профиля регистрации планирует применять на устройство во время следующего регистрации|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|Профиль регистрации времени была назначена на устройство|
|isSupervised|Boolean|Указывает, если управляет устройства Apple. Дополнительные сведения о был создан:https://support.apple.com/en-us/HT202837|
|discoverySource;|[discoverySource](../resources/intune-enrollment-discoverysource.md);|Источник обнаружения устройства Apple. Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|createdDateTime|DateTimeOffset|Время создания даты устройства|
|lastContactedDateTime|DateTimeOffset|Связаться с даты последнего устройства|
|описание|Строка|Описание устройства|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Состояние устройства в Intune. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|[Платформа](../resources/intune-enrollment-platform.md)|Платформа устройства. Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|

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
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```





