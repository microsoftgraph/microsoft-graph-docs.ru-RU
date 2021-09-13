---
title: тип ресурса windowsAutopilotDeviceIdentity
description: Ресурс windowsAutopilotDeviceIdentity представляет собой устройство Windows автопилота.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bd481a0b527e9665e145a48a23b41b6a2aab24f6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59028921"
---
# <a name="windowsautopilotdeviceidentity-resource-type"></a>тип ресурса windowsAutopilotDeviceIdentity

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс windowsAutopilotDeviceIdentity представляет собой устройство Windows автопилота.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsAutopilotDeviceIdentities](../api/intune-enrollment-windowsautopilotdeviceidentity-list.md)|[коллекция windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Список свойств и связей объектов [windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|
|[Get windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Чтение свойств и связей объекта [windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|
|[Создание объекта windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-create.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Создание нового [объекта windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|
|[Удаление windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-delete.md)|Нет|Удаляет [объект windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|
|[Действие assignUserToDevice](../api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice.md)|Нет|Назначает пользователя устройствам автопилота.|
|[Действие unassignUserFromDevice](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice.md)|Нет|Отписка пользователя с устройства Автопилота.|
|[действие updateDeviceProperties](../api/intune-enrollment-windowsautopilotdeviceidentity-updatedeviceproperties.md)|Нет|Обновляет свойства на устройствах автопилота.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID объекта|
|groupTag|Строка|Тег группы устройства Windows автопилота.|
|purchaseOrderIdentifier|Строка|Покупка идентификатора заказа устройства Windows автопилота.|
|serialNumber|Строка|Серийный номер устройства Windows Autopilot.|
|productKey|Строка|Ключ продукта устройства Windows Autopilot.|
|manufacturer|String|Oem производитель устройства Windows автопилота.|
|model|String|Имя модели устройства Windows автопилота.|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Состояние регистрации intune устройства Windows автопилота. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`.|
|lastContactedDateTime|DateTimeOffset|Intune Last Contacted Date Time of the Windows автопилота.|
|addressableUserName|Строка|Адресное имя пользователя.|
|userPrincipalName|String|Имя главного пользователя.|
|resourceName|String|Имя ресурса.|
|skuNumber|Строка|Номер SKU|
|systemFamily|Строка|Семейство system|
|azureActiveDirectoryDeviceId|Строка|AAD Device ID - to be deprecated|
|managedDeviceId|Строка|Управляемый ID устройства|
|displayName|String|"Display Name" (Отображаемое имя);|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "String (identifier)",
  "groupTag": "String",
  "purchaseOrderIdentifier": "String",
  "serialNumber": "String",
  "productKey": "String",
  "manufacturer": "String",
  "model": "String",
  "enrollmentState": "String",
  "lastContactedDateTime": "String (timestamp)",
  "addressableUserName": "String",
  "userPrincipalName": "String",
  "resourceName": "String",
  "skuNumber": "String",
  "systemFamily": "String",
  "azureActiveDirectoryDeviceId": "String",
  "managedDeviceId": "String",
  "displayName": "String"
}
```




