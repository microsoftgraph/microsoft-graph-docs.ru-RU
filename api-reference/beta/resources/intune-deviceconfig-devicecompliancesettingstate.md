---
title: Тип ресурса deviceComplianceSettingState
description: Состояние параметров соответствия требованиям для определенного устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9b1e428b7c17b5547ca6acfca467eead4bb7e2d8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526662"
---
# <a name="devicecompliancesettingstate-resource-type"></a>Тип ресурса deviceComplianceSettingState

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние параметров соответствия требованиям для определенного устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|Коллекция [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|Список свойств и связей объектов [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).|
|[Получение объекта deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md);|Чтение свойств и связей объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).|
|[Создание объекта deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md);|Создание объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).|
|[Удаление объекта deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|Нет|Удаляет объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).|
|[Обновление объекта deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|Обновление свойств объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта|
|platformType|[deviceType](../resources/intune-shared-devicetype.md)|Тип платформы устройства. Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry` `palm` `iSocConsumer` `unknown`,,,,,,,,,,,,,,,,,,,,,,,,. `winEmbedded` `iPhone` `iPad` `iPod` `android`|
|setting|String|Имя класса параметров и свойства.|
|settingName|String|Имя параметра в отчете|
|deviceId|String|ИД устройства в отчете|
|deviceName|String|Имя устройства в отчете|
|userId|String|ИД пользователя в отчете|
|userEmail|String|Электронный адрес пользователя в отчете|
|userName|String|Имя пользователя в отчете|
|userPrincipalName|String|Имя участника-пользователя в отчете|
|deviceModel|String|Модель устройства в отчете|
|state|[комплианцестатус](../resources/intune-shared-compliancestatus.md)|Состояние соответствия для параметра. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Дата и время истечения льготного периода соответствия требования для устройства|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "String (identifier)",
  "platformType": "String",
  "setting": "String",
  "settingName": "String",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userEmail": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "deviceModel": "String",
  "state": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)"
}
```



