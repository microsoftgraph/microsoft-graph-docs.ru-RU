---
title: Тип ресурса Виндовсинформатионпротектиондевицерегистратион
description: Представляет записи регистрации устройств для устройств Windows с поддержкой собственных устройств (BYOD).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dfdcd206f9a26e68e36f83e8c87e191e59612ebe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967877"
---
# <a name="windowsinformationprotectiondeviceregistration-resource-type"></a>Тип ресурса Виндовсинформатионпротектиондевицерегистратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет записи регистрации устройств для устройств Windows с поддержкой собственных устройств (BYOD).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсинформатионпротектиондевицерегистратионс](../api/intune-mam-windowsinformationprotectiondeviceregistration-list.md)|Коллекция [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Список свойств и связей объектов [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .|
|[Получение Виндовсинформатионпротектиондевицерегистратион](../api/intune-mam-windowsinformationprotectiondeviceregistration-get.md)|[Виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Чтение свойств и связей объекта [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .|
|[Создание Виндовсинформатионпротектиондевицерегистратион](../api/intune-mam-windowsinformationprotectiondeviceregistration-create.md)|[Виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Создание нового объекта [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .|
|[Удаление Виндовсинформатионпротектиондевицерегистратион](../api/intune-mam-windowsinformationprotectiondeviceregistration-delete.md)|Нет|Удаляет объект [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).|
|[Обновление Виндовсинформатионпротектиондевицерегистратион](../api/intune-mam-windowsinformationprotectiondeviceregistration-update.md)|[Виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Обновление свойств объекта [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .|
|[Действие wipe](../api/intune-mam-windowsinformationprotectiondeviceregistration-wipe.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|userId|String|UserId, связанный с этой записью регистрации устройства.|
|deviceRegistrationId|Строка|Идентификатор устройства для записи регистрации этого устройства.|
|deviceName|String|Имя устройства.|
|deviceType|String|Тип устройства, например Windows для портативного компьютера Windows и Windows Phone.|
|Девицемакаддресс|String|Mac-адрес устройства.|
|Ластчеккиндатетиме|DateTimeOffset|Время последнего возврата устройства.|

## <a name="relationships"></a>Отношения
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





