---
title: Тип ресурса windowsUpdateForBusinessConfiguration
description: Конфигурация Центра обновления Windows для бизнеса.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ccdcc7eb12f956669a82471734b5f99827467fd8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397031"
---
# <a name="windowsupdateforbusinessconfiguration-resource-type"></a>Тип ресурса windowsUpdateForBusinessConfiguration

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация Центра обновления Windows для бизнеса.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление windowsUpdateForBusinessConfigurations](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-list.md)|Коллекция [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)|Перечисление свойств и связей объектов [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).|
|[Получение windowsUpdateForBusinessConfiguration](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-get.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)|Считывание свойств и связей объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).|
|[Создание windowsUpdateForBusinessConfiguration](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-create.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)|Создание нового объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).|
|[Удаление windowsUpdateForBusinessConfiguration](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-delete.md)|None|Удаление экземпляра [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).|
|[Обновление windowsUpdateForBusinessConfiguration](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-update.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)|Обновление свойств объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).|
|[Действие extendFeatureUpdatesPause](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendfeatureupdatespause.md)|Нет|Расширение приостановить обновлений компонент для обновления Windows для бизнеса звонить.|
|[Действие extendQualityUpdatesPause](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendqualityupdatespause.md)|Нет|Расширьте приостановить качества обновления для обновления Windows для бизнеса звонка.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список областей теги для данного экземпляра сущности. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Логический|Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия. Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью. Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure. Это свойство доступно только для чтения. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deliveryOptimizationMode|[windowsDeliveryOptimizationMode](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|Режим оптимизации доставки. Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.|
|prereleaseFeatures|[prereleaseFeatures](../resources/intune-deviceconfig-prereleasefeatures.md)|Экспериментальные функции. Возможные значения: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.|
|automaticUpdateMode|[automaticUpdateMode](../resources/intune-deviceconfig-automaticupdatemode.md)|Режим автоматического обновления. Возможные значения: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.|
|microsoftUpdateServiceAllowed|Boolean|Разрешение использования службы обновлений (Майкрософт).|
|driversExcluded|Boolean|Исключение драйверов из Центра обновления Windows.|
|installationSchedule|[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|Расписание установки.|
|qualityUpdatesDeferralPeriodInDays|Int32|Откладывание исправлений на заданное количество дней.|
|featureUpdatesDeferralPeriodInDays|Int32|Откладывание обновлений компонентов на заданное количество дней.|
|qualityUpdatesPaused|Boolean|Приостановка исправлений.|
|featureUpdatesPaused|Boolean|Приостановка обновлений компонентов.|
|qualityUpdatesPauseExpiryDateTime|DateTimeOffset|Дата и время завершения срока приостановки исправлений.|
|featureUpdatesPauseExpiryDateTime|DateTimeOffset|Дата и время, когда будет завершен срок приостановки обновлений компонентов.|
|businessReadyUpdatesOnly|[windowsUpdateType](../resources/intune-deviceconfig-windowsupdatetype.md)|Определяет, какие устройства филиала будет получать обновления из. Возможные значения: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.|
|skipChecksBeforeRestart|Логический|Задайте для всех проверку перед перезагрузкой: уровень батарей = 40%, сведения о присутствии пользователя необходимости отображения, режиме презентации, полноэкранный режим, состояние телефонный звонок, режим игры и т.д. |
|updateWeeks|[windowsUpdateForBusinessUpdateWeeks](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|Планирование установки обновления на недели, месяца. Возможные значения: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.|
|qualityUpdatesPauseStartDate|дата;|Дата начала обновления приостановить качества. Это свойство доступно только для чтения.|
|featureUpdatesPauseStartDate|дата;|Дата начала приостановить обновления компонента. Это свойство доступно только для чтения.|
|featureUpdatesRollbackWindowInDays|Int32|Число дней после обновления компонента, для которого отката является допустимым|
|qualityUpdatesWillBeRolledBack|Логический|Определяет, будет ли отката обновлений качества на следующего устройства проверку|
|featureUpdatesWillBeRolledBack|Логический|Определяет, нужно ли выполнить откат обновления компонента на следующего устройства проверку|
|qualityUpdatesRollbackStartDateTime|DateTimeOffset|Качество запуск отката обновления даты и времени|
|featureUpdatesRollbackStartDateTime|DateTimeOffset|Запуск отката обновления даты и времени в функциях|
|engagedRestartDeadlineInDays|Int32|Крайний срок в днях, прежде чем автоматически планирование и выполнение отложенная перезагрузка active часы с допустимый диапазон от 2 до 30 дней|
|engagedRestartSnoozeScheduleInDays|Int32|Количество дней, пользователь может отложить выполняет перезапуск почте напоминания с допустимые значения от 1 до 3 дней|
|engagedRestartTransitionScheduleInDays|Int32|Количество дней до переход от автоматически перезапустит вне active часов выполняет перезапуск, с помощью которого пользователь может планировать с допустимый диапазон: от 0 до 30 дней|
|autoRestartNotificationDismissal|[autoRestartNotificationDismissalMethod](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|Выбор метода, с помощью которого перезапуск обязательные закрытия уведомлений. Возможные значения: `notConfigured`, `automatic`, `user`.|
|scheduleRestartWarningInHours|Int32|Укажите период для напоминания о автоматическую перезагрузку предупреждений. Поддерживаемые значения: 2, 4, 8, 12 или 24 (в часах).|
|scheduleImminentRestartWarningInMinutes|Int32|Укажите период для автоматическую перезагрузку предстоящее предупреждений. Поддерживаемые значения: 15, 30 или 60 (в минутах).|
|userPauseAccess|[Включение] (.. /Resources/Intune-Shared-enablement
публикацию повторно)|Указывает, следует ли включить доступа конечных пользователей для приостановки обновлений программного обеспечения. Возможные значения: `notConfigured`, `enabled`, `disabled`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) коллекции|Список назначений групп для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateForBusinessConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "deliveryOptimizationMode": "String",
  "prereleaseFeatures": "String",
  "automaticUpdateMode": "String",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "String",
    "scheduledInstallTime": "String (time of day)"
  },
  "qualityUpdatesDeferralPeriodInDays": 1024,
  "featureUpdatesDeferralPeriodInDays": 1024,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "String (timestamp)",
  "featureUpdatesPauseExpiryDateTime": "String (timestamp)",
  "businessReadyUpdatesOnly": "String",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "String",
  "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesRollbackWindowInDays": 1024,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "String (timestamp)",
  "featureUpdatesRollbackStartDateTime": "String (timestamp)",
  "engagedRestartDeadlineInDays": 1024,
  "engagedRestartSnoozeScheduleInDays": 1024,
  "engagedRestartTransitionScheduleInDays": 1024,
  "autoRestartNotificationDismissal": "String",
  "scheduleRestartWarningInHours": 1024,
  "scheduleImminentRestartWarningInMinutes": 1024,
  "userPauseAccess": "String"
}
```




