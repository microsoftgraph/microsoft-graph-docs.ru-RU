---
title: Тип ресурса Импортеддевицеидентити
description: Ресурс Импортеддевицеидентити представляет уникальное аппаратное удостоверение устройства, которое было предварительно подготовлено для настройки предварительной регистрации.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f5dcc3d7ef6cb59bffe1d7b8cfda958e76c3e35
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30572105"
---
# <a name="importeddeviceidentity-resource-type"></a>Тип ресурса Импортеддевицеидентити

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс Импортеддевицеидентити представляет уникальное аппаратное удостоверение устройства, которое было предварительно подготовлено для настройки предварительной регистрации.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Импортеддевицеидентитиес](../api/intune-enrollment-importeddeviceidentity-list.md)|Коллекция [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|Список свойств и связей объектов [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Получение Импортеддевицеидентити](../api/intune-enrollment-importeddeviceidentity-get.md)|[Импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|Чтение свойств и связей объекта [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Создание Импортеддевицеидентити](../api/intune-enrollment-importeddeviceidentity-create.md)|[Импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|Создание нового объекта [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Удаление Импортеддевицеидентити](../api/intune-enrollment-importeddeviceidentity-delete.md)|Нет|Удаляет объект [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md).|
|[Обновление Импортеддевицеидентити](../api/intune-enrollment-importeddeviceidentity-update.md)|[Импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|Обновление свойств объекта [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Действие importDeviceIdentityList](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|Коллекция [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md)|Пока не задокументировано.|
|[действие Сеарчексистингидентитиес](../api/intune-enrollment-importeddeviceidentity-searchexistingidentities.md)|Коллекция [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор импортированного удостоверения устройства|
|Импортеддевицеидентифиер|Строка|Импортированный идентификатор устройства|
|Импортеддевицеидентититипе|[Импортеддевицеидентититипе](../resources/intune-enrollment-importeddeviceidentitytype.md)|Тип импортированного удостоверения устройства. Возможные значения: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения описания|
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




