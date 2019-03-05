---
title: Тип ресурса windows10CompliancePolicy
description: Этот класс содержит параметры обеспечения соответствия требованиям для Windows 10.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 21f0c0e41f63979ab8e9d4a2ff2a649af9de1d97
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155974"
---
# <a name="windows10compliancepolicy-resource-type"></a>Тип ресурса windows10CompliancePolicy

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Этот класс содержит параметры обеспечения соответствия требованиям для Windows 10.


Наследуется от [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление windows10CompliancePolicies](../api/intune-deviceconfig-windows10compliancepolicy-list.md)|Коллекция [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)|Список свойств и связей объектов [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).|
|[Получение windows10CompliancePolicy](../api/intune-deviceconfig-windows10compliancepolicy-get.md)|[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md);|Считывание свойств и связей объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).|
|[Создание windows10CompliancePolicy](../api/intune-deviceconfig-windows10compliancepolicy-create.md)|[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md);|Создание объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).|
|[Удаление windows10CompliancePolicy](../api/intune-deviceconfig-windows10compliancepolicy-delete.md)|None|Удаление экземпляра [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).|
|[Обновление windows10CompliancePolicy](../api/intune-deviceconfig-windows10compliancepolicy-update.md)|[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)|Обновление свойств объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|id|String|Ключ объекта. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|description|Строка|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|passwordRequired|Логический|Указывает, что для разблокировки устройства с Windows требуется пароль.|
|passwordBlockSimple|Логический|Указывает, требуется ли блокировать простой пароль.|
|passwordRequiredToUnlockFromIdle|Логический|Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.|
|passwordMinutesOfInactivityBeforeLock|Int32|Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.|
|passwordExpirationDays|Int32|Срок действия пароля (в днях).|
|passwordMinimumLength|Int32|Минимальная длина пароля.|
|passwordMinimumCharacterSetCount|Int32|Количество наборов символов, которые требуются для пароля.|
|passwordRequiredType|[Рекуиредпассвордтипе](../resources/intune-deviceconfig-requiredpasswordtype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, повторное использование которых требуется запретить.|
|requireHealthyDeviceReport|Boolean|Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.|
|osMinimumVersion|String|Минимальная версия Windows 10.|
|osMaximumVersion|String|Максимальная версия Windows 10.|
|mobileOsMinimumVersion|String|Минимальная версия Windows Phone.|
|mobileOsMaximumVersion|String|Максимальная версия Windows Phone.|
|earlyLaunchAntiMalwareDriverEnabled|Логический|Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).|
|bitLockerEnabled|Логический|Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (средство BitLocker включено).|
|secureBootEnabled|Логический|Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (безопасная загрузка включена).|
|codeIntegrityEnabled|Boolean|Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности.|
|storageRequireEncryption|Логический|Указывает, обязательно ли шифрование данных на устройствах с Windows.|
|Свойства activefirewallrequired|Логический|Требуется активный брандмауэр на устройствах Windows.|
|Дефендеренаблед|Логический|Требуется антивредоносная программа защитника Windows на устройствах Windows.|
|Дефендерверсион|String|Требовать минимальную версию защиты от вредоносных программ Защитника Windows на устройствах Windows.|
|Сигнатуреаутофдате|Логический|Обязательное обновление подписи антивредоносной программы защитника Windows на устройствах Windows.|
|Ртпенаблед|Логический|Требование защиты от вредоносных программ Защитника Windows в режиме реального времени на устройствах Windows.|
|Антивирусрекуиред|Логический|Требование наличия антиВирусных решений, зарегистрированных в Windows Декурити Center для включения и отслеживания (например, Symantec, защитник Windows).|
|Антиспиваререкуиред|Логический|Обязательное решение для защиты от шпионских программ, зарегистрированное в Windows Декурити Center для включения и мониторинга (например, Symantec, защитник Windows).|
|validOperatingSystemBuildRanges|Коллекция [оператингсистемверсионранже](../resources/intune-deviceconfig-operatingsystemversionrange.md)|Допустимые диапазоны сборки операционной системы на устройствах Windows. Эта коллекция может содержать не более 10 000 элементов.|
|deviceThreatProtectionEnabled|Boolean|Указывает, что защита от угроз для устройств должна быть включена.|
|deviceThreatProtectionRequiredSecurityLevel|[Девицесреатпротектионлевел](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|ПоТребовать минимального уровня риска для защиты от угроз для отчетов о несоответствии. Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.|
|Конфигуратионманажеркомплианцерекуиред|Логический|Необходимо учитывать состояние соответствия SCCM в отношении состояния соответствия Intune.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|scheduledActionsForRule|Коллекция [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|Список запланированных действий для этого правила. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|deviceStatuses|Коллекция объектов [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)|Список DeviceComplianceDeviceStatus. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|userStatuses|Коллекция объектов [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|Список DeviceComplianceUserStatus. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|Обзор состояния обеспечения соответствия требованиям для устройств. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|Обзор состояния обеспечения соответствия требованиям для устройств, указанного для пользователей. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки обеспечения соответствия требованиям для устройств. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|assignments|Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|Коллекция назначений для этой политики соответствия требованиям. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10CompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "passwordPreviousPasswordBlockCount": 1024,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "mobileOsMinimumVersion": "String",
  "mobileOsMaximumVersion": "String",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "String",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "String",
      "lowestVersion": "String",
      "highestVersion": "String"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "configurationManagerComplianceRequired": true
}
```




