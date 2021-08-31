---
title: тип ресурса windowsInformationProtectionWipeAction
description: Представляет запросы на стирку, выданные администратором клиента для устройств Bring-Your-Own-Device (BYOD) Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aac1b49d6c2fab449fda91bdb5a339099950530e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786946"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a>тип ресурса windowsInformationProtectionWipeAction

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет запросы на стирку, выданные администратором клиента для устройств Bring-Your-Own-Device (BYOD) Windows.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsInformationProtectionWipeActions](../api/intune-mam-windowsinformationprotectionwipeaction-list.md)|[коллекция windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Список свойств и связей [объектов windowsInformationProtectionWipeAction.](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|
|[Получить windowsInformationProtectionWipeAction](../api/intune-mam-windowsinformationprotectionwipeaction-get.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Чтение свойств и связей [объекта windowsInformationProtectionWipeAction.](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|
|[Создание windowsInformationProtectionWipeAction](../api/intune-mam-windowsinformationprotectionwipeaction-create.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Создание нового [объекта windowsInformationProtectionWipeAction.](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|
|[Удаление windowsInformationProtectionWipeAction](../api/intune-mam-windowsinformationprotectionwipeaction-delete.md)|Нет|Удаляет [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).|
|[Обновление windowsInformationProtectionWipeAction](../api/intune-mam-windowsinformationprotectionwipeaction-update.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Обновление свойств объекта [windowsInformationProtectionWipeAction.](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|status|[actionState](../resources/intune-shared-actionstate.md)|Wipe action status. Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|targetedUserId|Строка|Объект UserId, на который нацелено это действие стирки.|
|targetedDeviceRegistrationId|Строка|Объект DeviceRegistrationId, нацеленный этим действием на стирку.|
|targetedDeviceName|Строка|Целевое имя устройства.|
|targetedDeviceMacAddress|Строка|Адрес Mac целевого устройства.|
|lastCheckInDateTime|DateTimeOffset|Время последней проверки устройства, на которое было нацелено это действие стирки.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionWipeAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "String (identifier)",
  "status": "String",
  "targetedUserId": "String",
  "targetedDeviceRegistrationId": "String",
  "targetedDeviceName": "String",
  "targetedDeviceMacAddress": "String",
  "lastCheckInDateTime": "String (timestamp)"
}
```



