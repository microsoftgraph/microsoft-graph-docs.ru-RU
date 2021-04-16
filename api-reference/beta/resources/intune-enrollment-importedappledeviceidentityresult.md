---
title: тип ресурса importedAppleDeviceIdentityResult
description: Ресурс importedAppleDeviceIdentityResult представляет собой результат попытки импорта удостоверений устройств Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 48b6acfe33009f349ba458f1afacc3f8701cadac
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868171"
---
# <a name="importedappledeviceidentityresult-resource-type"></a>тип ресурса importedAppleDeviceIdentityResult

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс importedAppleDeviceIdentityResult представляет собой результат попытки импорта удостоверений устройств Apple.


Наследуется [от импортируемого объектаAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список импортируемыхAppleDeviceIdentityResults](../api/intune-enrollment-importedappledeviceidentityresult-list.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection|Список свойств и связей импортируемых [объектовAppleDeviceIdentityResult.](../resources/intune-enrollment-importedappledeviceidentityresult.md)|
|[Получить importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-get.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).|Чтение свойств и связей импортируемого [объектаAppleDeviceIdentityResult.](../resources/intune-enrollment-importedappledeviceidentityresult.md)|
|[Создание importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-create.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).|Создание нового [объекта importedAppleDeviceIdentityResult.](../resources/intune-enrollment-importedappledeviceidentityresult.md)|
|[Удаление импортируемогоAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-delete.md)|Нет|Удаляет [импортируемуюAppleDeviceIdentityResult.](../resources/intune-enrollment-importedappledeviceidentityresult.md)|
|[Обновление importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-update.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).|Обновление свойств импортируемого [объектаAppleDeviceIdentityResult.](../resources/intune-enrollment-importedappledeviceidentityresult.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Унаследованный от [импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|serialNumber|String|Серийный номер устройства, унаследованный от [импортируемого ОбъектаAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|requestedEnrollmentProfileId|String|Администратор ID профиля регистрации намерен применить к устройству во время следующей регистрации, унаследованной от [импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|Профиль времени регистрации назначен устройству, унаследованной от [импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|isSupervised|Boolean|Указывает, контролируется ли устройство Apple. Дополнительные сведения: https://support.apple.com/en-us/HT202837 Унаследованные от [импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md);|Источник обнаружения устройств Apple. Наследуется [от импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md). Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|isDeleted|Логический|Указывает, удалено ли устройство из подразделения Apple Business Manager, унаследованной от [импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|createdDateTime|DateTimeOffset|Создано время даты устройства, унаследованной от [импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|lastContactedDateTime|DateTimeOffset|Время последней контактируемой даты устройства, унаследованной от [импортируемого ОбъектаAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|description|String|Описание устройства, унаследованной от [импортируемого ОбъектаAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Состояние устройства в Intune Наследуется от [импортируемогоAppleDeviceIdentity.](../resources/intune-enrollment-importedappledeviceidentity.md) Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|платформа|[платформа](../resources/intune-enrollment-platform.md)|Платформа устройства. Наследуется [от импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md). Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|status|Логический|Состояние удостоверения импортируемого устройства|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedAppleDeviceIdentityResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
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
  "platform": "String",
  "status": true
}
```




