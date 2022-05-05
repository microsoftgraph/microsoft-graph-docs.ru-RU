---
title: Обновление zebraFotaConnector
description: Обновление свойств объекта zebraFotaConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f38c88548649d462747dd1df0aa56df23276a66d
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213252"
---
# <a name="update-zebrafotaconnector"></a>Обновление zebraFotaConnector

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/zebraFotaConnector
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте представление объекта [zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md) в формате JSON.

В следующей таблице показаны свойства, необходимые при создании [zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор ZebraFotaConnector.|
|state|[zebraFotaConnectorState](../resources/intune-androidfotaservice-zebrafotaconnectorstate.md)|Состояние соединителя Zebra. Возможные значения: `none`, `connected`, `disconnected`, `unknownFutureValue`.|
|enrollmentToken|Строка|Маркер регистрации клиента от Zebra. Маркер используется для регистрации устройств Zebra в службе FOTA с помощью конфигурации приложения.|
|enrollmentAuthorizationUrl|Строка|Полный URL-адрес авторизации регистрации учетной записи. Это соответствует verification_uri_complete документации по API Zebra.|
|lastSyncDateTime|DateTimeOffset|Дата и время последней синхронизации учетной записи с Zebra|
|fotaAppsApproved|Логическое|Флаг, указывающий, утверждены ли необходимые приложения встроенного ПО по беспроводной сети (FOTA).|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код `200 OK` отклика и обновленный объект [zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/zebraFotaConnector
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.zebraFotaConnector",
  "state": "connected",
  "enrollmentToken": "Enrollment Token value",
  "enrollmentAuthorizationUrl": "https://example.com/enrollmentAuthorizationUrl/",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "fotaAppsApproved": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.zebraFotaConnector",
  "id": "2301310a-310a-2301-0a31-01230a310123",
  "state": "connected",
  "enrollmentToken": "Enrollment Token value",
  "enrollmentAuthorizationUrl": "https://example.com/enrollmentAuthorizationUrl/",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "fotaAppsApproved": true
}
```




