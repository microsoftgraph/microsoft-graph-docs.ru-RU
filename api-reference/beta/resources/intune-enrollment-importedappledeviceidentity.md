---
title: Тип ресурса Импортедаппледевицеидентити
description: Ресурс Импортедаппледевицеидентити представляет импортированное удостоверение устройства Apple.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 66b782c2402db03059c9487b50d0c49a8108e4bd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580298"
---
# <a name="importedappledeviceidentity-resource-type"></a>Тип ресурса Импортедаппледевицеидентити

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс Импортедаппледевицеидентити представляет импортированное удостоверение устройства Apple.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список importedAppleDeviceIdentities](../api/intune-enrollment-importedappledeviceidentity-list.md)|Коллекция [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|Список свойств и связей объектов [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Получение Импортедаппледевицеидентити](../api/intune-enrollment-importedappledeviceidentity-get.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Чтение свойств и связей объекта [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Создание Импортедаппледевицеидентити](../api/intune-enrollment-importedappledeviceidentity-create.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Создание нового объекта [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Удаление Импортедаппледевицеидентити](../api/intune-enrollment-importedappledeviceidentity-delete.md)|Нет|Удаляет объект [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md).|
|[Обновление Импортедаппледевицеидентити](../api/intune-enrollment-importedappledeviceidentity-update.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Обновление свойств объекта [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Действие importAppleDeviceIdentityList](../api/intune-enrollment-importedappledeviceidentity-importappledeviceidentitylist.md)|Коллекция [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|serialNumber|String|Серийный номер устройства|
|Рекуестеденроллментпрофилеид|String|Идентификатор профиля регистрации администратор планирует применить к устройству во время следующей регистрации|
|Рекуестеденроллментпрофилеассигнментдатетиме|DateTimeOffset|Для устройства назначен профиль регистрации времени.|
|isSupervised|Boolean|Указывает, защищено ли устройство Apple. Дополнительные сведения:https://support.apple.com/en-us/HT202837|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md);|Источник обнаружения устройств Apple. Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|createdDateTime|DateTimeOffset|Дата и время создания устройства|
|Ластконтактеддатетиме|DateTimeOffset|Дата и время последнего обращения к устройству|
|description|String|Описание устройства|
|Енроллментстате|[Енроллментстате](../resources/intune-enrollment-enrollmentstate.md)|Состояние устройства в Intune. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|[управляем](../resources/intune-enrollment-platform.md)|Платформа устройства. Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|

## <a name="relationships"></a>Отношения
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





