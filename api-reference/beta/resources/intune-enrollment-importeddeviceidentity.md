---
title: Тип ресурса Импортеддевицеидентити
description: Ресурс Импортеддевицеидентити представляет уникальное аппаратное удостоверение устройства, которое было предварительно подготовлено для настройки предварительной регистрации.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ca0c87fdd68f541d4645d0657123dafc73a11fb7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460828"
---
# <a name="importeddeviceidentity-resource-type"></a>Тип ресурса Импортеддевицеидентити

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс Импортеддевицеидентити представляет уникальное аппаратное удостоверение устройства, которое было предварительно подготовлено для настройки предварительной регистрации.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Импортеддевицеидентитиес](../api/intune-enrollment-importeddeviceidentity-list.md)|Коллекция [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|Список свойств и связей объектов [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Получение Импортеддевицеидентити](../api/intune-enrollment-importeddeviceidentity-get.md)|[импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|Чтение свойств и связей объекта [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Создание Импортеддевицеидентити](../api/intune-enrollment-importeddeviceidentity-create.md)|[импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|Создание нового объекта [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Удаление Импортеддевицеидентити](../api/intune-enrollment-importeddeviceidentity-delete.md)|Нет|Удаляет объект [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md).|
|[Обновление Импортеддевицеидентити](../api/intune-enrollment-importeddeviceidentity-update.md)|[импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|Обновление свойств объекта [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Действие importDeviceIdentityList](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|Коллекция [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md)|Пока не задокументировано.|
|[Действие searchExistingIdentities](../api/intune-enrollment-importeddeviceidentity-searchexistingidentities.md)|Коллекция [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор импортированного удостоверения устройства|
|импортеддевицеидентифиер|String|Импортированный идентификатор устройства|
|импортеддевицеидентититипе|[импортеддевицеидентититипе](../resources/intune-enrollment-importeddeviceidentitytype.md)|Тип импортированного удостоверения устройства. Возможные значения: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения описания|
|createdDateTime|DateTimeOffset|Дата и время создания устройства|
|ластконтактеддатетиме|DateTimeOffset|Дата и время последнего обращения к устройству|
|description|String|Описание устройства|
|енроллментстате|[енроллментстате](../resources/intune-shared-enrollmentstate.md)|Состояние устройства в Intune. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|[управляем](../resources/intune-enrollment-platform.md)|Платформа устройства. Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|

## <a name="relationships"></a>Отношения
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



