---
title: Получение Онпременкриптедпайлоад
description: Чтение свойств и связей объекта Онпременкриптедпайлоад.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ea86f77bb29418f3acb8f79afc65ec5eccba13b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741507"
---
# <a name="get-onpremencryptedpayload"></a><span data-ttu-id="b2651-103">Получение Онпременкриптедпайлоад</span><span class="sxs-lookup"><span data-stu-id="b2651-103">Get onPremEncryptedPayload</span></span>

> <span data-ttu-id="b2651-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2651-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2651-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2651-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2651-106">Чтение свойств и связей объекта [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) .</span><span class="sxs-lookup"><span data-stu-id="b2651-106">Read properties and relationships of the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2651-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b2651-107">Prerequisites</span></span>
<span data-ttu-id="b2651-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2651-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2651-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2651-110">Permission type</span></span>|<span data-ttu-id="b2651-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2651-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2651-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2651-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2651-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2651-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b2651-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2651-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2651-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2651-115">Not supported.</span></span>|
|<span data-ttu-id="b2651-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2651-116">Application</span></span>|<span data-ttu-id="b2651-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2651-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2651-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2651-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b2651-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b2651-119">Optional query parameters</span></span>
<span data-ttu-id="b2651-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b2651-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b2651-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2651-121">Request headers</span></span>
|<span data-ttu-id="b2651-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2651-122">Header</span></span>|<span data-ttu-id="b2651-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b2651-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2651-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2651-124">Authorization</span></span>|<span data-ttu-id="b2651-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2651-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2651-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b2651-126">Accept</span></span>|<span data-ttu-id="b2651-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b2651-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2651-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b2651-128">Request body</span></span>
<span data-ttu-id="b2651-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2651-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2651-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2651-130">Response</span></span>
<span data-ttu-id="b2651-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b2651-131">If successful, this method returns a `200 OK` response code and [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2651-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b2651-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2651-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2651-133">Request</span></span>
<span data-ttu-id="b2651-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2651-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
```

### <a name="response"></a><span data-ttu-id="b2651-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2651-135">Response</span></span>
<span data-ttu-id="b2651-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2651-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 834

{
  "value": {
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
}
```





