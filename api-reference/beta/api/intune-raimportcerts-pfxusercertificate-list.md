---
title: Список Пфксусерцертификатес
description: Список свойств и связей объектов Пфксусерцертификате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 45e55204a55da5a65b9d81731f64af3f6a8d245f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437677"
---
# <a name="list-pfxusercertificates"></a><span data-ttu-id="52b2a-103">Список Пфксусерцертификатес</span><span class="sxs-lookup"><span data-stu-id="52b2a-103">List pfxUserCertificates</span></span>

<span data-ttu-id="52b2a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52b2a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52b2a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52b2a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52b2a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52b2a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52b2a-107">Список свойств и связей объектов [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="52b2a-107">List properties and relationships of the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52b2a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="52b2a-108">Prerequisites</span></span>
<span data-ttu-id="52b2a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52b2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52b2a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52b2a-111">Permission type</span></span>|<span data-ttu-id="52b2a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="52b2a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52b2a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52b2a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52b2a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="52b2a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="52b2a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52b2a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52b2a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52b2a-116">Not supported.</span></span>|
|<span data-ttu-id="52b2a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52b2a-117">Application</span></span>|<span data-ttu-id="52b2a-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="52b2a-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52b2a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52b2a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /pfxUserCertificates
```

## <a name="request-headers"></a><span data-ttu-id="52b2a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="52b2a-120">Request headers</span></span>
|<span data-ttu-id="52b2a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52b2a-121">Header</span></span>|<span data-ttu-id="52b2a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="52b2a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52b2a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52b2a-123">Authorization</span></span>|<span data-ttu-id="52b2a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52b2a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52b2a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="52b2a-125">Accept</span></span>|<span data-ttu-id="52b2a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52b2a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52b2a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="52b2a-127">Request body</span></span>
<span data-ttu-id="52b2a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52b2a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52b2a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="52b2a-129">Response</span></span>
<span data-ttu-id="52b2a-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52b2a-130">If successful, this method returns a `200 OK` response code and a collection of [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52b2a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="52b2a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="52b2a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="52b2a-132">Request</span></span>
<span data-ttu-id="52b2a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52b2a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/pfxUserCertificates
```

### <a name="response"></a><span data-ttu-id="52b2a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="52b2a-134">Response</span></span>
<span data-ttu-id="52b2a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52b2a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



