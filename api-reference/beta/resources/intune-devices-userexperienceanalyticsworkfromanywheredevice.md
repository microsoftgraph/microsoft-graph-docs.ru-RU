---
title: тип ресурса userExperienceAnalyticsWorkFromAnywhereDevice
description: Устройство аналитики пользовательских интерфейсов для работы из любого отчета
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bd7db7eadfb9f14128c4bbfbbb69f69f881a1cec
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783934"
---
# <a name="userexperienceanalyticsworkfromanywheredevice-resource-type"></a>тип ресурса userExperienceAnalyticsWorkFromAnywhereDevice

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Устройство аналитики пользовательских интерфейсов для работы из любого отчета

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsWorkFromAnywhereDevices](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-list.md)|[коллекция userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|Список свойств и связей [объектов userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|
|[Get userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-get.md)|[userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|Чтение свойств и связей [объекта userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|
|[Создание userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-create.md)|[userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|Создание нового [объекта userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|
|[Удаление userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md).|
|[Обновление userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-update.md)|[userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|Обновление свойств объекта [userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор аналитики пользовательских интерфейсов работает с любого устройства.|
|deviceName|String|Работа из любого имени устройства.|
|serialNumber|String|Пользовательский интерфейс работает с любого серийного номера устройства.|
|manufacturer|String|Пользовательский интерфейс работает с любого производителя устройства.|
|model|String|Пользовательский интерфейс работает из любой модели устройства.|
|владение|String|Пользовательский интерфейс работает с любого владельца устройства.|
|managedBy|String|Пользовательский интерфейс работает из любого агента управления устройства.|
|autoPilotRegistered|Логический|Пользовательский интерфейс работает с автопилотом устройства intune.|
|autoPilotProfileAssigned|Логический|Аналитика пользовательских интерфейсов работает из любого автопилота устройства intuneProfileAssigned.|
|azureAdRegistered|Логический|Пользовательский интерфейс работает с azureAdRegistered любого устройства.|
|azureAdDeviceId|Строка|Пользовательский интерфейс работает из любого id-устройства Azure Ad.|
|azureAdJoinType|String|Пользовательский опыт работы из любого устройства azure Ad joinType.|
|osDescription|String|Пользовательский интерфейс работает из любого описания ОС устройства.|
|osVersion|String|Пользовательский интерфейс работает из любой версии ОС устройства.|
|tenantAttached|Boolean|Пользовательский интерфейс работает с любого клиента устройстваAttached.|
|compliancePolicySetToIntune|Логический|Пользовательский интерфейс работает из любой точки устройства compliancePolicySetToIntune.|
|otherWorkloadsSetToIntune|Логический|Пользовательский интерфейс работает из любого другого устройстваWorkloadsSetToIntune.|
|upgradeEligibility|[operatingSystemUpgradeEligibility](../resources/intune-devices-operatingsystemupgradeeligibility.md)|Пользовательский опыт работы из любой точки windows обновить состояние приемлемости устройства. Возможные значения: `upgraded`, `unknown`, `notCapable`, `capable`.|
|ramCheckFailed|Логический|Является ли работа аналитики пользовательского интерфейса из любой точки проверки оборудования оперативной памяти устройства неудачной для устройства для обновления до последней версии windows|
|storageCheckFailed|Логический|Пользовательский опыт работы с любого устройства, Является ли проверка оборудования хранения не удалось для устройства для обновления до последней версии windows.|
|processorCoreCountCheckFailed|Логический|Работа пользовательского интерфейса с любого устройства— проверка подсчета ядра процессора не удалось для устройства, чтобы обновиться до последней версии windows.|
|processorSpeedCheckFailed|Логический|Пользовательский опыт работы с любого устройства, Является ли проверка скорости оборудования процессора не удалось для устройства для обновления до последней версии windows.|
|tpmCheckFailed|Логический|Работа пользовательского интерфейса с любого устройства — это проверка аппаратного модуля доверенных платформ (TPM) для устройства до последней версии обновления до windows.|
|secureBootCheckFailed|Логический|Пользовательский опыт работы с любого устройства, является безопасной проверки оборудования загрузки не удалось для устройства для обновления до последней версии windows.|
|processorFamilyCheckFailed|Логический|Пользовательский опыт работы с любого устройства, является проверка семейства оборудования процессора не удалось для устройства для обновления до последней версии windows.|
|processor64BitCheckFailed|Логический|Пользовательский опыт работы с любого устройства, является ли проверка архитектуры процессорного оборудования 64-битной не удалось для устройства, чтобы обновить до последней версии windows.|
|osCheckFailed|Логический|Пользовательский опыт работы с любого устройства, является ли проверка ОС не удалось для устройства для обновления до последней версии windows.|
|WindowsScore|Двойное с плавающей точкой|Пользовательский интерфейс работает из любой точки на счет windows устройства. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|cloudManagementScore|Двойное с плавающей точкой|Пользовательский интерфейс работает из любой точки за оценку облачного управления устройствами. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|cloudIdentityScore|Двойное с плавающей точкой|Пользовательский опыт работы из любой точки за счет облачного удостоверения устройства. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|cloudProvisioningScore|Двойное с плавающей точкой|Пользовательский интерфейс работает из любой точки на счет облачного обеспечения устройства. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Пользовательский интерфейс работает из любой точки на состояние здоровья устройства. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "id": "String (identifier)",
  "deviceName": "String",
  "serialNumber": "String",
  "manufacturer": "String",
  "model": "String",
  "ownership": "String",
  "managedBy": "String",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdDeviceId": "String",
  "azureAdJoinType": "String",
  "osDescription": "String",
  "osVersion": "String",
  "tenantAttached": true,
  "compliancePolicySetToIntune": true,
  "otherWorkloadsSetToIntune": true,
  "upgradeEligibility": "String",
  "ramCheckFailed": true,
  "storageCheckFailed": true,
  "processorCoreCountCheckFailed": true,
  "processorSpeedCheckFailed": true,
  "tpmCheckFailed": true,
  "secureBootCheckFailed": true,
  "processorFamilyCheckFailed": true,
  "processor64BitCheckFailed": true,
  "osCheckFailed": true,
  "windowsScore": "4.2",
  "cloudManagementScore": "4.2",
  "cloudIdentityScore": "4.2",
  "cloudProvisioningScore": "4.2",
  "healthStatus": "String"
}
```



