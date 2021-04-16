---
title: Get pfxUserCertificate
description: Чтение свойств и связей объекта pfxUserCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b9847ae2a3866d20eb82214d7ec61a3fc998c0ad
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868839"
---
# <a name="get-pfxusercertificate"></a><span data-ttu-id="ded49-103">Get pfxUserCertificate</span><span class="sxs-lookup"><span data-stu-id="ded49-103">Get pfxUserCertificate</span></span>

<span data-ttu-id="ded49-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ded49-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ded49-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ded49-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ded49-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ded49-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ded49-107">Чтение свойств и связей объекта [pfxUserCertificate.](../resources/intune-raimportcerts-pfxusercertificate.md)</span><span class="sxs-lookup"><span data-stu-id="ded49-107">Read properties and relationships of the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ded49-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ded49-108">Prerequisites</span></span>
<span data-ttu-id="ded49-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ded49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ded49-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ded49-111">Permission type</span></span>|<span data-ttu-id="ded49-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ded49-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ded49-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ded49-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ded49-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ded49-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ded49-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ded49-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ded49-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ded49-116">Not supported.</span></span>|
|<span data-ttu-id="ded49-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ded49-117">Application</span></span>|<span data-ttu-id="ded49-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ded49-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ded49-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ded49-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /pfxUserCertificates/{pfxUserCertificatesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ded49-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ded49-120">Optional query parameters</span></span>
<span data-ttu-id="ded49-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ded49-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ded49-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ded49-122">Request headers</span></span>
|<span data-ttu-id="ded49-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ded49-123">Header</span></span>|<span data-ttu-id="ded49-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ded49-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ded49-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ded49-125">Authorization</span></span>|<span data-ttu-id="ded49-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ded49-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ded49-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ded49-127">Accept</span></span>|<span data-ttu-id="ded49-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ded49-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ded49-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ded49-129">Request body</span></span>
<span data-ttu-id="ded49-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ded49-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ded49-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ded49-131">Response</span></span>
<span data-ttu-id="ded49-132">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ded49-132">If successful, this method returns a `200 OK` response code and [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ded49-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ded49-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ded49-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ded49-134">Request</span></span>
<span data-ttu-id="ded49-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ded49-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/pfxUserCertificates/{pfxUserCertificatesId}
```

### <a name="response"></a><span data-ttu-id="ded49-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ded49-136">Response</span></span>
<span data-ttu-id="ded49-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ded49-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 844

{
  "value": {
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
}
```




