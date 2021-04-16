---
title: Список onPremEncryptedPayloads
description: Список свойств и связей объектов onPremEncryptedPayload.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 08da9a9efa869d674ab90a676924a6f99853196a
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868770"
---
# <a name="list-onpremencryptedpayloads"></a><span data-ttu-id="e5bec-103">Список onPremEncryptedPayloads</span><span class="sxs-lookup"><span data-stu-id="e5bec-103">List onPremEncryptedPayloads</span></span>

<span data-ttu-id="e5bec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5bec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5bec-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5bec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5bec-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5bec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5bec-107">Список свойств и связей объектов [onPremEncryptedPayload.](../resources/intune-raimportcerts-onpremencryptedpayload.md)</span><span class="sxs-lookup"><span data-stu-id="e5bec-107">List properties and relationships of the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5bec-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e5bec-108">Prerequisites</span></span>
<span data-ttu-id="e5bec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5bec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5bec-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5bec-111">Permission type</span></span>|<span data-ttu-id="e5bec-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5bec-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5bec-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5bec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5bec-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5bec-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e5bec-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5bec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5bec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5bec-116">Not supported.</span></span>|
|<span data-ttu-id="e5bec-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="e5bec-117">Application</span></span>|<span data-ttu-id="e5bec-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5bec-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5bec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5bec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /onPremEncryptedPayloads
```

## <a name="request-headers"></a><span data-ttu-id="e5bec-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e5bec-120">Request headers</span></span>
|<span data-ttu-id="e5bec-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5bec-121">Header</span></span>|<span data-ttu-id="e5bec-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e5bec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5bec-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5bec-123">Authorization</span></span>|<span data-ttu-id="e5bec-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5bec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5bec-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e5bec-125">Accept</span></span>|<span data-ttu-id="e5bec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5bec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5bec-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5bec-127">Request body</span></span>
<span data-ttu-id="e5bec-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5bec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5bec-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5bec-129">Response</span></span>
<span data-ttu-id="e5bec-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e5bec-130">If successful, this method returns a `200 OK` response code and a collection of [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5bec-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e5bec-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5bec-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5bec-132">Request</span></span>
<span data-ttu-id="e5bec-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5bec-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/onPremEncryptedPayloads
```

### <a name="response"></a><span data-ttu-id="e5bec-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5bec-134">Response</span></span>
<span data-ttu-id="e5bec-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5bec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 882

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.onPremEncryptedPayload",
      "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
      "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
      "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
      "payloadId": "f12f6c03-6c03-f12f-036c-2ff1036c2ff1",
      "deviceKeyThumbprint": "Device Key Thumbprint value",
      "cert1PayloadUUID": "Cert1Payload UUID value",
      "cert2PayloadUUID": "Cert2Payload UUID value",
      "cert3PayloadUUID": "Cert3Payload UUID value",
      "plistTemplate": "Plist Template value",
      "encryptedBlob": "ZW5jcnlwdGVkQmxvYg==",
      "payloadVersion": 14,
      "status": 6,
      "createdTime": "2017-01-01T00:03:18.9597073-08:00",
      "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
      "eTag": "ETag value",
      "isDeleted": true
    }
  ]
}
```




