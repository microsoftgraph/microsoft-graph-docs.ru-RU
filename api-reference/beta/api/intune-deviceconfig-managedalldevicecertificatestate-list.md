---
title: Список managedAllDeviceCertificateStates
description: Список свойств и связей объектов managedAllDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4d3a558fbf3fc3c97563077f17d4ae99c65110bc
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58790775"
---
# <a name="list-managedalldevicecertificatestates"></a>Список managedAllDeviceCertificateStates

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей [объектов managedAllDeviceCertificateState.](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 958

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
      "id": "987c6a17-6a17-987c-176a-7c98176a7c98",
      "certificateRevokeStatus": "pending",
      "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:34.9547208-08:00",
      "managedDeviceDisplayName": "Managed Device Display Name value",
      "userPrincipalName": "User Principal Name value",
      "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
      "certificateIssuerName": "Certificate Issuer Name value",
      "certificateThumbprint": "Certificate Thumbprint value",
      "certificateSerialNumber": "Certificate Serial Number value",
      "certificateSubjectName": "Certificate Subject Name value",
      "certificateKeyUsages": 4,
      "certificateExtendedKeyUsages": "Certificate Extended Key Usages value",
      "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00"
    }
  ]
}
```



