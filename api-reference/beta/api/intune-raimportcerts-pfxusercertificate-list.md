---
title: Список Пфксусерцертификатес
description: Список свойств и связей объектов Пфксусерцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 98fea8274904816999928c9fbf5c4fa427bfbe5f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741482"
---
# <a name="list-pfxusercertificates"></a><span data-ttu-id="3a988-103">Список Пфксусерцертификатес</span><span class="sxs-lookup"><span data-stu-id="3a988-103">List pfxUserCertificates</span></span>

> <span data-ttu-id="3a988-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a988-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a988-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a988-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a988-106">Список свойств и связей объектов [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="3a988-106">List properties and relationships of the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a988-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3a988-107">Prerequisites</span></span>
<span data-ttu-id="3a988-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a988-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a988-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a988-110">Permission type</span></span>|<span data-ttu-id="3a988-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a988-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a988-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a988-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3a988-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a988-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3a988-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a988-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a988-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a988-115">Not supported.</span></span>|
|<span data-ttu-id="3a988-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a988-116">Application</span></span>|<span data-ttu-id="3a988-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a988-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a988-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a988-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /pfxUserCertificates
```

## <a name="request-headers"></a><span data-ttu-id="3a988-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a988-119">Request headers</span></span>
|<span data-ttu-id="3a988-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a988-120">Header</span></span>|<span data-ttu-id="3a988-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3a988-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a988-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a988-122">Authorization</span></span>|<span data-ttu-id="3a988-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a988-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a988-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3a988-124">Accept</span></span>|<span data-ttu-id="3a988-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3a988-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a988-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3a988-126">Request body</span></span>
<span data-ttu-id="3a988-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a988-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a988-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a988-128">Response</span></span>
<span data-ttu-id="3a988-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3a988-129">If successful, this method returns a `200 OK` response code and a collection of [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a988-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3a988-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a988-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a988-131">Request</span></span>
<span data-ttu-id="3a988-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a988-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/pfxUserCertificates
```

### <a name="response"></a><span data-ttu-id="3a988-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a988-133">Response</span></span>
<span data-ttu-id="3a988-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a988-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 894

{
  "value": [
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
  ]
}
```





