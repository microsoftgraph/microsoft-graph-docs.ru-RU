---
title: Обновление объекта deviceManagementPartner
description: Обновление свойств объекта deviceManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c8e9425968d00805eb8640ff3a7e19380a92c6dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838782"
---
# <a name="update-devicemanagementpartner"></a>Обновление объекта deviceManagementPartner

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Обновление свойств объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).
## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте представление объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в формате JSON.

Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Н/Д|
|lastHeartbeatDateTime|DateTimeOffset|Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".|
|partnerState|[deviceManagementPartnerTenantState](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|Состояние партнера клиента. Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.|
|partnerAppType|[deviceManagementPartnerAppType](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|Партнерские типа приложения. Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.|
|singleTenantAppId|String|Идентификатор одноклиентского приложения партнера|
|displayName|String|Отображаемое имя партнера|
|isConfigured|Boolean|Указывает, настроен ли партнер по управлению устройствами|
|whenPartnerDevicesWillBeRemovedDateTime|DateTimeOffset|Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства.|
|whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime|DateTimeOffset|Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям.|



## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 502

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 551

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```



