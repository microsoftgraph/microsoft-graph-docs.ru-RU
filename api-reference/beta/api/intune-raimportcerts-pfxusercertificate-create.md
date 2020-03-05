---
title: Создание Пфксусерцертификате
description: Создание нового объекта Пфксусерцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bac316037c22a2a26d6331d32771895cbb6c7db1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460096"
---
# <a name="create-pfxusercertificate"></a>Создание Пфксусерцертификате

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxUserCertificates
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта Пфксусерцертификате в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Пфксусерцертификате.

|Свойство|Тип|Описание|
|:---|:---|:---|
|tenantId|GUID|Пока не задокументировано.|
|userId|GUID|Пока не задокументировано.|
|отпечаток|String|Пока не задокументировано.|
|усерупн|String|Пока не задокументировано.|
|енкриптедпфксблоб|String|Пока не задокументировано.|
|енкриптедпфкспассворд|String|Пока не задокументировано.|
|цертстартдате|DateTimeOffset|Пока не задокументировано.|
|цертекспиратиондате|DateTimeOffset|Пока не задокументировано.|
|providerName|String|Пока не задокументировано.|
|енкриптионкэйнаме|String|Пока не задокументировано.|
|паддингсчеме|Int32|Пока нет описания|
|status|Int32|Пока нет описания|
|intendedPurpose|Int32|Пока нет описания|
|createdTime|DateTimeOffset|Пока не задокументировано.|
|isDeleted|Boolean|Пока не задокументировано|
|lastModifiedTime|DateTimeOffset|Пока не задокументировано.|
|eTag|String|Пока не задокументировано.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/pfxUserCertificates
Content-type: application/json
Content-length: 789

{
  "@odata.type": "#microsoft.graph.pfxUserCertificate",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "thumbprint": "Thumbprint value",
  "userUpn": "User Upn value",
  "encryptedPfxBlob": "Encrypted Pfx Blob value",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "certStartDate": "2017-01-01T00:01:48.7697664-08:00",
  "certExpirationDate": "2016-12-31T23:56:39.3841403-08:00",
  "providerName": "Provider Name value",
  "encryptionKeyName": "Encryption Key Name value",
  "paddingScheme": 13,
  "status": 6,
  "intendedPurpose": 15,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "isDeleted": true,
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 789

{
  "@odata.type": "#microsoft.graph.pfxUserCertificate",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "thumbprint": "Thumbprint value",
  "userUpn": "User Upn value",
  "encryptedPfxBlob": "Encrypted Pfx Blob value",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "certStartDate": "2017-01-01T00:01:48.7697664-08:00",
  "certExpirationDate": "2016-12-31T23:56:39.3841403-08:00",
  "providerName": "Provider Name value",
  "encryptionKeyName": "Encryption Key Name value",
  "paddingScheme": 13,
  "status": 6,
  "intendedPurpose": 15,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "isDeleted": true,
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value"
}
```





