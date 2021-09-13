---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: rolyon
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3f2829a759266b4b0254077df78740a3f5394beb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59132591"
---
# <a name="update-devicemanagement"></a>Обновление объекта deviceManagement

Пространство имен: microsoft.graph

> **Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).

## <a name="prerequisites"></a>Предварительные условия

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

Обратите внимание, что разрешение зависит от рабочего процесса.

| Тип &nbsp; разрешения &nbsp; &nbsp; (по рабочего процесса) | Разрешения (в порядке убывания привилегий) |
|:---|:---|
| Делегированные (рабочая или учебная учетная запись) ||
| &nbsp;&nbsp; **Android для работы** | DeviceManagementConfiguration.ReadWrite.All  |
| &nbsp; &nbsp; **Аудит** | DeviceManagementApps.ReadWrite.All |
| &nbsp; &nbsp; **Условия компании** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **Конфигурация устройства** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp; **Намерение устройства** | DeviceManagementConfiguration.ReadWrite.All|
| &nbsp; &nbsp; **Управление устройствами** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; **Электронная SIM-карта** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp; **Регистрация** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Фехтования** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp; &nbsp; **Уведомление** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Odj** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **Адаптация** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Набор политик** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)** | DeviceManagementRBAC.ReadWrite.All |
| &nbsp;&nbsp; **Удаленный доступ** | DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **Удаленная помощь** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **Обновление программного обеспечения** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Управление расходами телекома** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Troublehooting** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp; &nbsp; **Windows Information Protection** | DeviceManagementApps.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.|
| Для приложений ||
| &nbsp;&nbsp; **Android для работы** | DeviceManagementConfiguration.ReadWrite.All  |
| &nbsp; &nbsp; **Аудит** | DeviceManagementApps.ReadWrite.All |
| &nbsp; &nbsp; **Условия компании** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **Конфигурация устройства** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp; **Намерение устройства** | DeviceManagementConfiguration.ReadWrite.All|
| &nbsp; &nbsp; **Управление устройствами** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; **Электронная SIM-карта** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp; **Регистрация** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Фехтования** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp; &nbsp; **Уведомление** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Odj** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **Адаптация** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Набор политик** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)** | DeviceManagementRBAC.ReadWrite.All |
| &nbsp;&nbsp; **Удаленный доступ** | DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **Удаленная помощь** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **Обновление программного обеспечения** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Управление расходами телекома** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Troublehooting** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp; &nbsp; **Windows Information Protection** | DeviceManagementApps.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a>Заголовки запроса

|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса

В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.

В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для устройства.|
|**Конфигурация устройств**|
|intuneAccountId|GUID|ID учетной записи Intune для данного клиента|
|legacyPcManangementEnabled|Логическое|Свойство, чтобы включить для этой учетной записи управление устаревшим КОМПЬЮТЕРом без MDM. Это свойство доступно только для чтения.|
|maximumDepTokens|Int32|Максимальное количество маркеров DEP, разрешенных для каждого клиента.|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Параметры уровня учетной записи.|
|**Управление устройствами**|
|accountMoveCompletionDateTime|DateTimeOffset|Дата &, когда данные клиента перемещаются между scaleunits.|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|Сведения о согласии администратора.|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md);|Обзор защиты устройств.|
|managedDeviceCleanupSettings;|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md);|Правило очистки устройств|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Состояние подписки на управление мобильными устройствами для клиента. Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|subscriptions|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|Подписка клиента. Возможные значения: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Обзор вредоносных программ для устройств Windows.|
|**Адаптация**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.|

Поддержка свойств тела запроса зависит от рабочего процесса.

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Вот пример запроса, следующего за процессом управления устройствами:

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика. 

Примечание. Представленный здесь объект отклика может быть усечен для краткости. Возвращенные свойства различаются в зависимости от рабочего процесса и контекста.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```









