---
title: Тип ресурса Импортедаппледевицеидентитиресулт
description: Ресурс Импортедаппледевицеидентитиресулт представляет результат попытки импорта удостоверений устройств Apple.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d286e49f7b073f5deb6163a06f7641fe16f3347
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799337"
---
# <a name="importedappledeviceidentityresult-resource-type"></a>Тип ресурса Импортедаппледевицеидентитиресулт

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс Импортедаппледевицеидентитиресулт представляет результат попытки импорта удостоверений устройств Apple.


НаСледуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Импортедаппледевицеидентитиресултс](../api/intune-enrollment-importedappledeviceidentityresult-list.md)|Коллекция [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md)|Список свойств и связей объектов [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) .|
|[Получение Импортедаппледевицеидентитиресулт](../api/intune-enrollment-importedappledeviceidentityresult-get.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|Чтение свойств и связей объекта [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) .|
|[Создание Импортедаппледевицеидентитиресулт](../api/intune-enrollment-importedappledeviceidentityresult-create.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|Создание нового объекта [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) .|
|[Удаление Импортедаппледевицеидентитиресулт](../api/intune-enrollment-importedappledeviceidentityresult-delete.md)|Нет|Удаляет объект [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md).|
|[Обновление Импортедаппледевицеидентитиресулт](../api/intune-enrollment-importedappledeviceidentityresult-update.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|Обновление свойств объекта [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. НаСледуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|serialNumber|String|Серийный номер устройства, наСледуемый от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|Рекуестеденроллментпрофилеид|String|Идентификатор профиля регистрации администратор планирует применить к устройству во время следующей регистрации, унаследованной от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|Рекуестеденроллментпрофилеассигнментдатетиме|DateTimeOffset|Профиль регистрации времени назначен устройству, унаследованному от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|isSupervised|Boolean|Указывает, защищено ли устройство Apple. Дополнительные сведения: https://support.apple.com/en-us/HT202837 наследуются от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Источник обнаружения устройств Apple. НаСледуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md). Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|createdDateTime|DateTimeOffset|Дата и время создания устройства, унаследованного от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|Ластконтактеддатетиме|DateTimeOffset|Дата и время последнего обращения к устройству, унаследованному от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|description|String|Описание устройства, наСледуемого из [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|Енроллментстате|[Енроллментстате](../resources/intune-enrollment-enrollmentstate.md)|Состояние устройства в Intune, наСледуемого из [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md). Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|[platform](../resources/intune-enrollment-platform.md)|Платформа устройства. НаСледуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md). Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|status|Boolean|Состояние импортированного удостоверения устройства|

## <a name="relationships"></a>Отношения
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
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String",
  "status": true
}
```





