---
title: Список Пфксусерцертификатес
description: Список свойств и связей объектов Пфксусерцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 08daeac4951b23d45a67ded6dd024d8fc22b719a
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161546"
---
# <a name="list-pfxusercertificates"></a><span data-ttu-id="db7dc-103">Список Пфксусерцертификатес</span><span class="sxs-lookup"><span data-stu-id="db7dc-103">List pfxUserCertificates</span></span>

> <span data-ttu-id="db7dc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db7dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db7dc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db7dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db7dc-106">Список свойств и связей объектов [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="db7dc-106">List properties and relationships of the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db7dc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="db7dc-107">Prerequisites</span></span>
<span data-ttu-id="db7dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db7dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db7dc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db7dc-110">Permission type</span></span>|<span data-ttu-id="db7dc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="db7dc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db7dc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db7dc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db7dc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="db7dc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="db7dc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db7dc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db7dc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db7dc-115">Not supported.</span></span>|
|<span data-ttu-id="db7dc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db7dc-116">Application</span></span>|<span data-ttu-id="db7dc-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="db7dc-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db7dc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db7dc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /pfxUserCertificates
```

## <a name="request-headers"></a><span data-ttu-id="db7dc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="db7dc-119">Request headers</span></span>
|<span data-ttu-id="db7dc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="db7dc-120">Header</span></span>|<span data-ttu-id="db7dc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="db7dc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db7dc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db7dc-122">Authorization</span></span>|<span data-ttu-id="db7dc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db7dc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db7dc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="db7dc-124">Accept</span></span>|<span data-ttu-id="db7dc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="db7dc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db7dc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db7dc-126">Request body</span></span>
<span data-ttu-id="db7dc-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db7dc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db7dc-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="db7dc-128">Response</span></span>
<span data-ttu-id="db7dc-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="db7dc-129">If successful, this method returns a `200 OK` response code and a collection of [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db7dc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="db7dc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="db7dc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="db7dc-131">Request</span></span>
<span data-ttu-id="db7dc-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db7dc-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/pfxUserCertificates
```

### <a name="response"></a><span data-ttu-id="db7dc-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="db7dc-133">Response</span></span>
<span data-ttu-id="db7dc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db7dc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





