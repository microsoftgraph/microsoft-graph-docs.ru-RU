---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f4ef1c7eb4711afd2aa29071f160f440dceefba3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415777"
---
# <a name="update-devicemanagement"></a>Обновление объекта deviceManagement

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).

## <a name="prerequisites"></a>Предварительные условия

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

Обратите внимание, что это разрешение различаться в зависимости от рабочего процесса.

| Разрешение&nbsp;тип&nbsp;(с&nbsp;рабочего процесса) | Разрешения (в порядке убывания привилегий) |
|:---|:---|
| Делегированные (рабочая или учебная учетная запись) ||
| &nbsp;&nbsp; **Android для работы** | DeviceManagementConfiguration.ReadWrite.All  |
| &nbsp; &nbsp; **аудита;** | DeviceManagementApps.ReadWrite.All |
| &nbsp;&nbsp; **Компании термины** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Конфигурация устройств** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp; &nbsp; **Управление устройствами** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; **Электронных диспетчера установки** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp; &nbsp; **Регистрация** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Разграничения** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp; &nbsp; **Уведомление** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Адаптация новых сотрудников** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Управления доступом на основе ролей (RBAC)** | DeviceManagementRBAC.ReadWrite.All |
| &nbsp;&nbsp; **Удаленного доступа** | DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **Удаленный помощник** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Управления расходами телекоммуникации** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Troublehooting** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; **Защита информации Windows** | DeviceManagementApps.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.|
| Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a>Заголовки запросов

|Заголовок|Значение|
|:---|:---|
|Authorization|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса

В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.

В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для устройства.|
|**Конфигурация устройств**|
|intuneAccountId|GUID|Идентификатор учетной записи Intune для заданного клиента|
|legacyPcManangementEnabled|Логический|Свойство для включения не MDM управляемых прежних версий управления ПК для этой учетной записи. Это свойство доступно только для чтения.|
|maximumDepTokens|Int32|Максимальное число DEP маркеры могут каждого клиента.|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Параметры уровня учетной записи.|
|**Управление устройствами**|
|accountMoveCompletionDateTime|DateTimeOffset|Время & даты, при перемещении данные клиента между ScaleUnits строкового.|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|Сведения о разрешения администратора.|
|deviceProtectionOverview;|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md);|Общие сведения о защите устройств.|
|managedDeviceCleanupSettings;|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md);|Правила очистки устройства|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Состояние подписки на управление мобильными устройствами для клиента. Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|подписки|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|Подписка клиента. Возможные значения: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Обзор вредоносных программ для устройств windows.|
|**Адаптация новых сотрудников**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.|

Поддержка свойств текст запроса изменяется в зависимости от рабочего процесса.

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса на следующий рабочий процесс управления устройств:

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

Примечание. Представленный здесь объект отклика может быть усечен для краткости. Возвращаемых свойств различаться в зависимости от рабочего процесса и контекста.

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



