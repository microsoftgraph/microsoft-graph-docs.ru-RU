---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 57fddece1d8059e46121f23596180636c5765913
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463823"
---
# <a name="update-devicemanagement"></a>Обновление объекта deviceManagement

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).

## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам) | Разрешения (в порядке убывания привилегий) |
|:---|:---|
| Делегированные (рабочая или учебная учетная запись) |
| &nbsp;&nbsp; Аудит | DeviceManagementApps.ReadWrite.All |
| &nbsp;&nbsp; Условия компании | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; Корпоративная регистрация | DeviceManagementServiceConfig.ReadWrite.All|
| &nbsp;&nbsp; Конфигурация устройства | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp; Управление устройствами | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; Endpoint Protection | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; Уведомление | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; Входящая миграция | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; Управление доступом на основе ролей | DeviceManagementRBAC.ReadWrite.All |
| &nbsp;&nbsp; Удаленная помощь | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; Управление расходами по телекоммуникационной связи | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; Устранение неполадок | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; Windows Information Protection | DeviceManagementApps.ReadWrite.All |
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

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.

В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор устройства.|
|**Конфигурация устройства**|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Параметры уровня учетной записи.|
|**Управление устройствами**|
|subscriptionState|[девицеманажементсубскриптионстате](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Состояние подписки на управление мобильными устройствами для клиента. Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|**Адаптация**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.|

Поддержка свойств текста запроса зависит от рабочего процесса.

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
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

Ниже приведен пример отклика. Примечание. Представленный здесь объект отклика может быть усечен для краткости. Возвращаемые свойства различаются в зависимости от рабочего процесса и контекста.

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






