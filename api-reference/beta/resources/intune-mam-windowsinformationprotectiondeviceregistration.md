---
title: Тип ресурса Виндовсинформатионпротектиондевицерегистратион
description: Представляет записи регистрации устройств для устройств Windows с поддержкой собственных устройств (BYOD).
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b7d30fad170fa03d96fbfb715d81dbdc028b776
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42780656"
---
# <a name="windowsinformationprotectiondeviceregistration-resource-type"></a>Тип ресурса Виндовсинформатионпротектиондевицерегистратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет записи регистрации устройств для устройств Windows с поддержкой собственных устройств (BYOD).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсинформатионпротектиондевицерегистратионс](../api/intune-mam-windowsinformationprotectiondeviceregistration-list.md)|Коллекция [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Список свойств и связей объектов [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .|
|[Получение Виндовсинформатионпротектиондевицерегистратион](../api/intune-mam-windowsinformationprotectiondeviceregistration-get.md)|[виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Чтение свойств и связей объекта [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .|
|[Создание Виндовсинформатионпротектиондевицерегистратион](../api/intune-mam-windowsinformationprotectiondeviceregistration-create.md)|[виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Создание нового объекта [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .|
|[Удаление Виндовсинформатионпротектиондевицерегистратион](../api/intune-mam-windowsinformationprotectiondeviceregistration-delete.md)|Нет|Удаляет объект [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).|
|[Обновление Виндовсинформатионпротектиондевицерегистратион](../api/intune-mam-windowsinformationprotectiondeviceregistration-update.md)|[виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Обновление свойств объекта [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .|
|[Действие wipe](../api/intune-mam-windowsinformationprotectiondeviceregistration-wipe.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|userId|String|UserId, связанный с этой записью регистрации устройства.|
|deviceRegistrationId|Строка|Идентификатор устройства для записи регистрации этого устройства.|
|deviceName|String|Имя устройства.|
|deviceType|String|Тип устройства, например Windows для портативного компьютера Windows и Windows Phone.|
|девицемакаддресс|String|Mac-адрес устройства.|
|ластчеккиндатетиме|DateTimeOffset|Время последнего возврата устройства.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDeviceRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "id": "String (identifier)",
  "userId": "String",
  "deviceRegistrationId": "String",
  "deviceName": "String",
  "deviceType": "String",
  "deviceMacAddress": "String",
  "lastCheckInDateTime": "String (timestamp)"
}
```



