---
title: тип ресурса windowsInformationProtectionDeviceRegistration
description: Представляет записи регистрации устройств для устройств Bring-Your-Own-Device (BYOD) Windows устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9cb3be503f401675ba286961e89f027b36219b8a
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58796848"
---
# <a name="windowsinformationprotectiondeviceregistration-resource-type"></a>тип ресурса windowsInformationProtectionDeviceRegistration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет записи регистрации устройств для устройств Bring-Your-Own-Device (BYOD) Windows устройств.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsInformationProtectionDeviceRegistrations](../api/intune-mam-windowsinformationprotectiondeviceregistration-list.md)|[коллекция windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Список свойств и связей объектов [windowsInformationProtectionDeviceRegistration.](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|
|[Получить windowsInformationProtectionDeviceRegistration](../api/intune-mam-windowsinformationprotectiondeviceregistration-get.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Чтение свойств и связей [объекта windowsInformationProtectionDeviceRegistration.](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|
|[Создание windowsInformationProtectionDeviceRegistration](../api/intune-mam-windowsinformationprotectiondeviceregistration-create.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Создание нового [объекта windowsInformationProtectionDeviceRegistration.](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|
|[Удаление windowsInformationProtectionDeviceRegistration](../api/intune-mam-windowsinformationprotectiondeviceregistration-delete.md)|Нет|Удаляет [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).|
|[Обновление windowsInformationProtectionDeviceRegistration](../api/intune-mam-windowsinformationprotectiondeviceregistration-update.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Обновление свойств объекта [windowsInformationProtectionDeviceRegistration.](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|
|[Действие wipe](../api/intune-mam-windowsinformationprotectiondeviceregistration-wipe.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|userId|String|UserId, связанный с этой записью регистрации устройства.|
|deviceRegistrationId|Строка|Идентификатор устройства для записи регистрации устройства.|
|deviceName|String|Имя устройства.|
|deviceType|String|Тип устройства, например, Windows ноутбук vs Windows телефон.|
|deviceMacAddress|Строка|Адрес Mac устройства.|
|lastCheckInDateTime|DateTimeOffset|Время последней проверки устройства.|

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



