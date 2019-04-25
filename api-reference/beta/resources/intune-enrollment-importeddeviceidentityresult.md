---
title: Тип ресурса Импортеддевицеидентитиресулт
description: Ресурс Импортеддевицеидентитиресулт представляет результат попытки импорта удостоверения устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b94eff5ea5e2ed37173341b45980e9b60437822d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524500"
---
# <a name="importeddeviceidentityresult-resource-type"></a>Тип ресурса Импортеддевицеидентитиресулт

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс Импортеддевицеидентитиресулт представляет результат попытки импорта удостоверения устройства.


НаСледуется от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Импортеддевицеидентитиресултс](../api/intune-enrollment-importeddeviceidentityresult-list.md)|Коллекция [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md)|Список свойств и связей объектов [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md) .|
|[Получение Импортеддевицеидентитиресулт](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[Импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md)|Чтение свойств и связей объекта [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md) .|
|[Создание Импортеддевицеидентитиресулт](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[Импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md)|Создание нового объекта [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md) .|
|[Удаление Импортеддевицеидентитиресулт](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|Нет|Удаляет объект [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md).|
|[Обновление Импортеддевицеидентитиресулт](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[Импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md)|Обновление свойств объекта [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор импортированного удостоверения устройства, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|
|Импортеддевицеидентифиер|String|Импортированный идентификатор устройства, наСледуемый от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|
|Импортеддевицеидентититипе|[Импортеддевицеидентититипе](../resources/intune-enrollment-importeddeviceidentitytype.md)|Тип импортированного удостоверения устройства, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md). Возможные значения: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения описания, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|
|createdDateTime|DateTimeOffset|Дата и время создания устройства, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|
|Ластконтактеддатетиме|DateTimeOffset|Дата и время последнего обращения к устройству, унаследованному от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|
|description|String|Описание устройства, наСледуемого из [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|
|Енроллментстате|[Енроллментстате](../resources/intune-enrollment-enrollmentstate.md)|Состояние устройства в Intune, наСледуемого из [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md). Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|[управляем](../resources/intune-enrollment-platform.md)|Платформа устройства. НаСледуется от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md). Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|status|Boolean|Состояние импортированного удостоверения устройства|

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





