---
title: Тип ресурса Импортеддевицеидентитиресулт
description: Ресурс Импортеддевицеидентитиресулт представляет результат попытки импорта удостоверения устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7efe3e69edccaf87d7025b667e798363feaa5f8e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256388"
---
# <a name="importeddeviceidentityresult-resource-type"></a>Тип ресурса Импортеддевицеидентитиресулт

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс Импортеддевицеидентитиресулт представляет результат попытки импорта удостоверения устройства.


Наследуется от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Импортеддевицеидентитиресултс](../api/intune-enrollment-importeddeviceidentityresult-list.md)|Коллекция [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md)|Список свойств и связей объектов [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md) .|
|[Получение Импортеддевицеидентитиресулт](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md)|Чтение свойств и связей объекта [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md) .|
|[Создание Импортеддевицеидентитиресулт](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md)|Создание нового объекта [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md) .|
|[Удаление Импортеддевицеидентитиресулт](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|Нет|Удаляет объект [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md).|
|[Обновление Импортеддевицеидентитиресулт](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md)|Обновление свойств объекта [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор импортированного удостоверения устройства, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|
|импортеддевицеидентифиер|String|Импортированный идентификатор устройства, наследуемый от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|
|импортеддевицеидентититипе|[импортеддевицеидентититипе](../resources/intune-enrollment-importeddeviceidentitytype.md)|Тип импортированного удостоверения устройства, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md). Возможные значения: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения описания, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|
|createdDateTime|DateTimeOffset|Дата и время создания устройства, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|
|ластконтактеддатетиме|DateTimeOffset|Дата и время последнего обращения к устройству, унаследованному от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|
|description|String|Описание устройства, наследуемого из [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|
|енроллментстате|[енроллментстате](../resources/intune-shared-enrollmentstate.md)|Состояние устройства в Intune, наследуемого из [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md). Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|платформа|[платформа](../resources/intune-enrollment-platform.md)|Платформа устройства. Наследуется от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md). Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|status|Boolean|Состояние импортированного удостоверения устройства|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentityResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String",
  "status": true
}
```




