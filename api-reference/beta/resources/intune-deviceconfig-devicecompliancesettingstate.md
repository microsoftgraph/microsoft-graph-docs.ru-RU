---
title: Тип ресурса deviceComplianceSettingState
description: Состояние параметров соответствия требованиям для определенного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4966683ce1a2a52def7773d5ef311bfccc8f9ddb
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670655"
---
# <a name="devicecompliancesettingstate-resource-type"></a>Тип ресурса deviceComplianceSettingState

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние параметров соответствия требованиям для определенного устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|Коллекция [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|Список свойств и связей объектов [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).|
|[Получение объекта deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|Чтение свойств и связей объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).|
|[Создание объекта deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|Создание объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).|
|[Удаление объекта deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|Нет|Удаляет объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).|
|[Обновление объекта deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|Обновление свойств объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта|
|platformType|[deviceType](../resources/intune-deviceconfig-devicetype.md)|Тип платформы устройства. Возможные значения: `desktop`, , `windowsRT``winMO6`, `nokia`, `windowsPhone`, `holoLens``macMDM``winCE``winEmbedded``mac``iPhone``iPod``android``iPad``androidForWork``unix``surfaceHub``iSocConsumer``androidEnterprise`, `chromeOS``windows10x``androidnGMS``linux`, , , `blackberry`, . `palm``unknown``cloudPC`|
|setting|String|Имя класса параметров и свойства.|
|settingName|String|Имя параметра в отчете|
|deviceId|String|ИД устройства в отчете|
|deviceName|String|Имя устройства в отчете|
|userId|String|ИД пользователя в отчете|
|userEmail|String|Электронный адрес пользователя в отчете|
|userName|String|Имя пользователя в отчете|
|userPrincipalName|String|Имя участника-пользователя в отчете|
|deviceModel|String|Модель устройства в отчете|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Состояние соответствия параметра. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
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




