---
title: Получение deviceManagement
description: Чтение свойств и связей объекта deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 96c7667e34812e34f1ddf12bc25425ffecc147a0
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940000"
---
# <a name="get-devicemanagement"></a>Получение deviceManagement

> **Важно!** API в версии/Beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Чтение свойств и связей объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).

## <a name="prerequisites"></a>Предварительные условия

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам) | Разрешения (в порядке убывания привилегий) |
|:---|:---|
| Делегированные (рабочая или учебная учетная запись) | |
| &nbsp;&nbsp; **Android для работы** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp; &nbsp; **Аудит** | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All |
| &nbsp; &nbsp; **Условия компании** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **Конфигурация устройства** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **Цель устройства** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
| &nbsp; &nbsp; **Управление устройствами** | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All |
| &nbsp;&nbsp; **Электронная SIM-карта** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **Регистрация** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **Ограждение** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp; &nbsp; **Уведомление** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **Одж** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **Адаптация** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **Набор политик** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **RBAC** | DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All |
| &nbsp; &nbsp; **Удаленный доступ** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **Удаленная помощь** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **Обновление программного обеспечения** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **Управление расходами по телекоммуникационной** связи | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **Устранение неполадок** | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All |
| &nbsp; &nbsp; **Windows Information Protection** | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.|
| Для приложений | |
| &nbsp;&nbsp; **Android для работы** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp; &nbsp; **Аудит** | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All |
| &nbsp; &nbsp; **Условия компании** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **Конфигурация устройства** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **Цель устройства** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
| &nbsp; &nbsp; **Управление устройствами** | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All |
| &nbsp;&nbsp; **Электронная SIM-карта** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **Регистрация** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **Ограждение** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp; &nbsp; **Уведомление** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **Одж** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **Адаптация** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **Набор политик** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **RBAC** | DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All |
| &nbsp; &nbsp; **Удаленный доступ** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **Удаленная помощь** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **Обновление программного обеспечения** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **Управление расходами по телекоммуникационной** связи | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **Устранение неполадок** | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All |
| &nbsp; &nbsp; **Windows Information Protection** | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All |

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика. 

Note: объекты ответа, показанные здесь, могут быть усечены для краткости.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```

Возвращаются свойства, подходящие для рабочего процесса.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
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
}
```











