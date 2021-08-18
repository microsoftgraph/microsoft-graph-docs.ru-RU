---
title: тип ресурса windowsInformationProtectionWipeAction
description: Представляет запросы на стирку, выданные администратором клиента для устройств Bring-Your-Own-Device (BYOD) Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0b03d1e13b02d4956c634932e8dee1e58818b25eb17c3ac585257b0209fa69fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54241557"
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
|id|String|Ключ объекта.|
|status|[actionState](../resources/intune-shared-actionstate.md)|Wipe action status. Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|targetedUserId|String|Объект UserId, на который нацелено это действие стирки.|
|targetedDeviceRegistrationId|String|Объект DeviceRegistrationId, нацеленный этим действием на стирку.|
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




