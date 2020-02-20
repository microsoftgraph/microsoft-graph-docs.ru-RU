---
title: Создание Онпременкриптедпайлоад
description: Создание нового объекта Онпременкриптедпайлоад.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c86aed4b4994258d0e2f44f574d3126e1aa2079e
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161321"
---
# <a name="create-onpremencryptedpayload"></a><span data-ttu-id="465a2-103">Создание Онпременкриптедпайлоад</span><span class="sxs-lookup"><span data-stu-id="465a2-103">Create onPremEncryptedPayload</span></span>

> <span data-ttu-id="465a2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="465a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="465a2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="465a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="465a2-106">Создание нового объекта [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) .</span><span class="sxs-lookup"><span data-stu-id="465a2-106">Create a new [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="465a2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="465a2-107">Prerequisites</span></span>
<span data-ttu-id="465a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="465a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="465a2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="465a2-110">Permission type</span></span>|<span data-ttu-id="465a2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="465a2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="465a2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="465a2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="465a2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="465a2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="465a2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="465a2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="465a2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="465a2-115">Not supported.</span></span>|
|<span data-ttu-id="465a2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="465a2-116">Application</span></span>|<span data-ttu-id="465a2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="465a2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="465a2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="465a2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /onPremEncryptedPayloads
```

## <a name="request-headers"></a><span data-ttu-id="465a2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="465a2-119">Request headers</span></span>
|<span data-ttu-id="465a2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="465a2-120">Header</span></span>|<span data-ttu-id="465a2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="465a2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="465a2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="465a2-122">Authorization</span></span>|<span data-ttu-id="465a2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="465a2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="465a2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="465a2-124">Accept</span></span>|<span data-ttu-id="465a2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="465a2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="465a2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="465a2-126">Request body</span></span>
<span data-ttu-id="465a2-127">В тексте запроса добавьте представление объекта Онпременкриптедпайлоад в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="465a2-127">In the request body, supply a JSON representation for the onPremEncryptedPayload object.</span></span>

<span data-ttu-id="465a2-128">В следующей таблице приведены свойства, необходимые при создании Онпременкриптедпайлоад.</span><span class="sxs-lookup"><span data-stu-id="465a2-128">The following table shows the properties that are required when you create the onPremEncryptedPayload.</span></span>

|<span data-ttu-id="465a2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="465a2-129">Property</span></span>|<span data-ttu-id="465a2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="465a2-130">Type</span></span>|<span data-ttu-id="465a2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="465a2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="465a2-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="465a2-132">tenantId</span></span>|<span data-ttu-id="465a2-133">GUID</span><span class="sxs-lookup"><span data-stu-id="465a2-133">Guid</span></span>|<span data-ttu-id="465a2-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="465a2-134">Not yet documented</span></span>|
|<span data-ttu-id="465a2-135">userId</span><span class="sxs-lookup"><span data-stu-id="465a2-135">userId</span></span>|<span data-ttu-id="465a2-136">GUID</span><span class="sxs-lookup"><span data-stu-id="465a2-136">Guid</span></span>|<span data-ttu-id="465a2-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="465a2-137">Not yet documented</span></span>|
|<span data-ttu-id="465a2-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="465a2-138">deviceId</span></span>|<span data-ttu-id="465a2-139">Guid</span><span class="sxs-lookup"><span data-stu-id="465a2-139">Guid</span></span>|<span data-ttu-id="465a2-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="465a2-140">Not yet documented</span></span>|
|<span data-ttu-id="465a2-141">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="465a2-141">payloadId</span></span>|<span data-ttu-id="465a2-142">GUID</span><span class="sxs-lookup"><span data-stu-id="465a2-142">Guid</span></span>|<span data-ttu-id="465a2-143">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="465a2-143">Not yet documented</span></span>|
|<span data-ttu-id="465a2-144">девицекэйсумбпринт</span><span class="sxs-lookup"><span data-stu-id="465a2-144">deviceKeyThumbprint</span></span>|<span data-ttu-id="465a2-145">String</span><span class="sxs-lookup"><span data-stu-id="465a2-145">String</span></span>|<span data-ttu-id="465a2-146">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="465a2-146">Not yet documented</span></span>|
|<span data-ttu-id="465a2-147">cert1PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="465a2-147">cert1PayloadUUID</span></span>|<span data-ttu-id="465a2-148">String</span><span class="sxs-lookup"><span data-stu-id="465a2-148">String</span></span>|<span data-ttu-id="465a2-149">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="465a2-149">Not yet documented</span></span>|
|<span data-ttu-id="465a2-150">cert2PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="465a2-150">cert2PayloadUUID</span></span>|<span data-ttu-id="465a2-151">String</span><span class="sxs-lookup"><span data-stu-id="465a2-151">String</span></span>|<span data-ttu-id="465a2-152">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="465a2-152">Not yet documented</span></span>|
|<span data-ttu-id="465a2-153">cert3PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="465a2-153">cert3PayloadUUID</span></span>|<span data-ttu-id="465a2-154">String</span><span class="sxs-lookup"><span data-stu-id="465a2-154">String</span></span>|<span data-ttu-id="465a2-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="465a2-155">Not yet documented</span></span>|
|<span data-ttu-id="465a2-156">плисттемплате</span><span class="sxs-lookup"><span data-stu-id="465a2-156">plistTemplate</span></span>|<span data-ttu-id="465a2-157">String</span><span class="sxs-lookup"><span data-stu-id="465a2-157">String</span></span>|<span data-ttu-id="465a2-158">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="465a2-158">Not yet documented</span></span>|
|<span data-ttu-id="465a2-159">енкриптедблоб</span><span class="sxs-lookup"><span data-stu-id="465a2-159">encryptedBlob</span></span>|<span data-ttu-id="465a2-160">Binary</span><span class="sxs-lookup"><span data-stu-id="465a2-160">Binary</span></span>|<span data-ttu-id="465a2-161">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="465a2-161">Not yet documented</span></span>|
|<span data-ttu-id="465a2-162">пайлоадверсион</span><span class="sxs-lookup"><span data-stu-id="465a2-162">payloadVersion</span></span>|<span data-ttu-id="465a2-163">Int32</span><span class="sxs-lookup"><span data-stu-id="465a2-163">Int32</span></span>|<span data-ttu-id="465a2-164">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="465a2-164">Not yet documented</span></span>|
|<span data-ttu-id="465a2-165">status</span><span class="sxs-lookup"><span data-stu-id="465a2-165">status</span></span>|<span data-ttu-id="465a2-166">Int32</span><span class="sxs-lookup"><span data-stu-id="465a2-166">Int32</span></span>|<span data-ttu-id="465a2-167">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="465a2-167">Not yet documented</span></span>|
|<span data-ttu-id="465a2-168">createdTime</span><span class="sxs-lookup"><span data-stu-id="465a2-168">createdTime</span></span>|<span data-ttu-id="465a2-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="465a2-169">DateTimeOffset</span></span>|<span data-ttu-id="465a2-170">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="465a2-170">Not yet documented</span></span>|
|<span data-ttu-id="465a2-171">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="465a2-171">lastModifiedTime</span></span>|<span data-ttu-id="465a2-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="465a2-172">DateTimeOffset</span></span>|<span data-ttu-id="465a2-173">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="465a2-173">Not yet documented</span></span>|
|<span data-ttu-id="465a2-174">eTag</span><span class="sxs-lookup"><span data-stu-id="465a2-174">eTag</span></span>|<span data-ttu-id="465a2-175">String</span><span class="sxs-lookup"><span data-stu-id="465a2-175">String</span></span>|<span data-ttu-id="465a2-176">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="465a2-176">Not yet documented</span></span>|
|<span data-ttu-id="465a2-177">isDeleted</span><span class="sxs-lookup"><span data-stu-id="465a2-177">isDeleted</span></span>|<span data-ttu-id="465a2-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="465a2-178">Boolean</span></span>|<span data-ttu-id="465a2-179">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="465a2-179">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="465a2-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="465a2-180">Response</span></span>
<span data-ttu-id="465a2-181">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="465a2-181">If successful, this method returns a `201 Created` response code and a [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="465a2-182">Пример</span><span class="sxs-lookup"><span data-stu-id="465a2-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="465a2-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="465a2-183">Request</span></span>
<span data-ttu-id="465a2-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="465a2-184">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/onPremEncryptedPayloads
Content-type: application/json
Content-length: 781

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
```

### <a name="response"></a><span data-ttu-id="465a2-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="465a2-185">Response</span></span>
<span data-ttu-id="465a2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="465a2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 781

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
```





