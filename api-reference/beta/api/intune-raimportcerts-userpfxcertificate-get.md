---
title: Get userPFXCertificate
description: Чтение свойств и связей объекта userPFXCertificate.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 070f7446e64ea23111828dba0ad7f6020e89afea
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59107465"
---
# <a name="get-userpfxcertificate"></a>Get userPFXCertificate

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Чтение свойств и связей [объекта userPFXCertificate.](../resources/intune-raimportcerts-userpfxcertificate.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и `200 OK` [объект userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 742

{
  "value": {
    "@odata.type": "#microsoft.graph.userPFXCertificate",
    "id": "045c159b-159b-045c-9b15-5c049b155c04",
    "thumbprint": "Thumbprint value",
    "intendedPurpose": "smimeEncryption",
    "userPrincipalName": "User Principal Name value",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "providerName": "Provider Name value",
    "keyName": "Key Name value",
    "paddingScheme": "pkcs1",
    "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
    "encryptedPfxPassword": "Encrypted Pfx Password value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```



