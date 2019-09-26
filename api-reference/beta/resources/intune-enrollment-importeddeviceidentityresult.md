---
title: Тип ресурса Импортеддевицеидентитиресулт
description: Ресурс Импортеддевицеидентитиресулт представляет результат попытки импорта удостоверения устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ea80061d9ebb14b53c97e9213f5b9bbc60091e78
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196604"
---
# <a name="importeddeviceidentityresult-resource-type"></a>Тип ресурса Импортеддевицеидентитиресулт

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|Строка|Идентификатор импортированного удостоверения устройства, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|
|импортеддевицеидентифиер|String.|Импортированный идентификатор устройства, наследуемый от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|
|импортеддевицеидентититипе|[импортеддевицеидентититипе](../resources/intune-enrollment-importeddeviceidentitytype.md)|Тип импортированного удостоверения устройства, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md). Возможные значения: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения описания, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|
|createdDateTime|DateTimeOffset|Дата и время создания устройства, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|
|ластконтактеддатетиме|DateTimeOffset|Дата и время последнего обращения к устройству, унаследованному от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|
|description|String|Описание устройства, наследуемого из [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|
|енроллментстате|[енроллментстате](../resources/intune-shared-enrollmentstate.md)|Состояние устройства в Intune, наследуемого из [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md). Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|[управляем](../resources/intune-enrollment-platform.md)|Платформа устройства. Наследуется от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md). Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|status|Boolean.|Состояние импортированного удостоверения устройства|

## <a name="relationships"></a>Отношения
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



