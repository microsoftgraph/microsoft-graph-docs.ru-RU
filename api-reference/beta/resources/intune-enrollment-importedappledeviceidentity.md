---
title: Тип ресурса Импортедаппледевицеидентити
description: Ресурс Импортедаппледевицеидентити представляет импортированное удостоверение устройства Apple.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 277ca83a4df6a3f8125fb3e2ae1687da6cef05ba
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941592"
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
|Рекуестеденроллментпрофилеид|Строка|Идентификатор профиля регистрации администратор планирует применить к устройству во время следующей регистрации|
|Рекуестеденроллментпрофилеассигнментдатетиме|DateTimeOffset|Для устройства назначен профиль регистрации времени.|
|isSupervised|Boolean|Указывает, защищено ли устройство Apple. Дополнительные сведения:https://support.apple.com/en-us/HT202837|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md);|Источник обнаружения устройств Apple. Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|createdDateTime|DateTimeOffset|Дата и время создания устройства|
|Ластконтактеддатетиме|DateTimeOffset|Дата и время последнего обращения к устройству|
|description|String|Описание устройства|
|Енроллментстате|[Енроллментстате](../resources/intune-enrollment-enrollmentstate.md)|Состояние устройства в Intune. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|[управляем](../resources/intune-enrollment-platform.md)|Платформа устройства. Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|

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




