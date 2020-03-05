---
title: Тип ресурса Импортедаппледевицеидентитиресулт
description: Ресурс Импортедаппледевицеидентитиресулт представляет результат попытки импорта удостоверений устройств Apple.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2a464e20880cf8c431e6f52e3413974b019007f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528296"
---
# <a name="importedappledeviceidentityresult-resource-type"></a>Тип ресурса Импортедаппледевицеидентитиресулт

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс Импортедаппледевицеидентитиресулт представляет результат попытки импорта удостоверений устройств Apple.


Наследуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Импортедаппледевицеидентитиресултс](../api/intune-enrollment-importedappledeviceidentityresult-list.md)|Коллекция [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md)|Список свойств и связей объектов [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) .|
|[Получение Импортедаппледевицеидентитиресулт](../api/intune-enrollment-importedappledeviceidentityresult-get.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).|Чтение свойств и связей объекта [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) .|
|[Создание Импортедаппледевицеидентитиресулт](../api/intune-enrollment-importedappledeviceidentityresult-create.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).|Создание нового объекта [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) .|
|[Удаление Импортедаппледевицеидентитиресулт](../api/intune-enrollment-importedappledeviceidentityresult-delete.md)|Нет|Удаляет объект [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md).|
|[Обновление Импортедаппледевицеидентитиресулт](../api/intune-enrollment-importedappledeviceidentityresult-update.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).|Обновление свойств объекта [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|serialNumber|String|Серийный номер устройства, наследуемый от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|рекуестеденроллментпрофилеид|String|Идентификатор профиля регистрации администратор планирует применить к устройству во время следующей регистрации, унаследованной от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|рекуестеденроллментпрофилеассигнментдатетиме|DateTimeOffset|Профиль регистрации времени назначен устройству, унаследованному от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|isSupervised|Boolean|Указывает, защищено ли устройство Apple. Дополнительные сведения: https://support.apple.com/en-us/HT202837 наследуются от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md);|Источник обнаружения устройств Apple. Наследуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md). Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|isDeleted|Логический|Указывает, будет ли устройство удалено из Apple Business Manager, унаследованное от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|createdDateTime|DateTimeOffset|Дата и время создания устройства, унаследованного от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|ластконтактеддатетиме|DateTimeOffset|Дата и время последнего обращения к устройству, унаследованному от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|description|String|Описание устройства, наследуемого из [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|енроллментстате|[енроллментстате](../resources/intune-shared-enrollmentstate.md)|Состояние устройства в Intune, наследуемого из [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md). Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|[управляем](../resources/intune-enrollment-platform.md)|Платформа устройства. Наследуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md). Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|status|Логический|Состояние импортированного удостоверения устройства|

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



