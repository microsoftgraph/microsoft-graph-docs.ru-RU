---
title: Создание Онпременкриптедпайлоад
description: Создание нового объекта Онпременкриптедпайлоад.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5c5a045a517fe5fc2b7d33ccf052be169114df89
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460180"
---
# <a name="create-onpremencryptedpayload"></a><span data-ttu-id="27f8b-103">Создание Онпременкриптедпайлоад</span><span class="sxs-lookup"><span data-stu-id="27f8b-103">Create onPremEncryptedPayload</span></span>

<span data-ttu-id="27f8b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="27f8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27f8b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27f8b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27f8b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27f8b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27f8b-107">Создание нового объекта [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) .</span><span class="sxs-lookup"><span data-stu-id="27f8b-107">Create a new [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27f8b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="27f8b-108">Prerequisites</span></span>
<span data-ttu-id="27f8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27f8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27f8b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27f8b-111">Permission type</span></span>|<span data-ttu-id="27f8b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="27f8b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27f8b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27f8b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27f8b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27f8b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="27f8b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27f8b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27f8b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27f8b-116">Not supported.</span></span>|
|<span data-ttu-id="27f8b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27f8b-117">Application</span></span>|<span data-ttu-id="27f8b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27f8b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27f8b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27f8b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /onPremEncryptedPayloads
```

## <a name="request-headers"></a><span data-ttu-id="27f8b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="27f8b-120">Request headers</span></span>
|<span data-ttu-id="27f8b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="27f8b-121">Header</span></span>|<span data-ttu-id="27f8b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="27f8b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27f8b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="27f8b-123">Authorization</span></span>|<span data-ttu-id="27f8b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27f8b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27f8b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="27f8b-125">Accept</span></span>|<span data-ttu-id="27f8b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27f8b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27f8b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27f8b-127">Request body</span></span>
<span data-ttu-id="27f8b-128">В тексте запроса добавьте представление объекта Онпременкриптедпайлоад в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27f8b-128">In the request body, supply a JSON representation for the onPremEncryptedPayload object.</span></span>

<span data-ttu-id="27f8b-129">В следующей таблице приведены свойства, необходимые при создании Онпременкриптедпайлоад.</span><span class="sxs-lookup"><span data-stu-id="27f8b-129">The following table shows the properties that are required when you create the onPremEncryptedPayload.</span></span>

|<span data-ttu-id="27f8b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="27f8b-130">Property</span></span>|<span data-ttu-id="27f8b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="27f8b-131">Type</span></span>|<span data-ttu-id="27f8b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="27f8b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27f8b-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="27f8b-133">tenantId</span></span>|<span data-ttu-id="27f8b-134">GUID</span><span class="sxs-lookup"><span data-stu-id="27f8b-134">Guid</span></span>|<span data-ttu-id="27f8b-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27f8b-135">Not yet documented</span></span>|
|<span data-ttu-id="27f8b-136">userId</span><span class="sxs-lookup"><span data-stu-id="27f8b-136">userId</span></span>|<span data-ttu-id="27f8b-137">GUID</span><span class="sxs-lookup"><span data-stu-id="27f8b-137">Guid</span></span>|<span data-ttu-id="27f8b-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27f8b-138">Not yet documented</span></span>|
|<span data-ttu-id="27f8b-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="27f8b-139">deviceId</span></span>|<span data-ttu-id="27f8b-140">Guid</span><span class="sxs-lookup"><span data-stu-id="27f8b-140">Guid</span></span>|<span data-ttu-id="27f8b-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27f8b-141">Not yet documented</span></span>|
|<span data-ttu-id="27f8b-142">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="27f8b-142">payloadId</span></span>|<span data-ttu-id="27f8b-143">GUID</span><span class="sxs-lookup"><span data-stu-id="27f8b-143">Guid</span></span>|<span data-ttu-id="27f8b-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27f8b-144">Not yet documented</span></span>|
|<span data-ttu-id="27f8b-145">девицекэйсумбпринт</span><span class="sxs-lookup"><span data-stu-id="27f8b-145">deviceKeyThumbprint</span></span>|<span data-ttu-id="27f8b-146">String</span><span class="sxs-lookup"><span data-stu-id="27f8b-146">String</span></span>|<span data-ttu-id="27f8b-147">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27f8b-147">Not yet documented</span></span>|
|<span data-ttu-id="27f8b-148">cert1PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="27f8b-148">cert1PayloadUUID</span></span>|<span data-ttu-id="27f8b-149">String</span><span class="sxs-lookup"><span data-stu-id="27f8b-149">String</span></span>|<span data-ttu-id="27f8b-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27f8b-150">Not yet documented</span></span>|
|<span data-ttu-id="27f8b-151">cert2PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="27f8b-151">cert2PayloadUUID</span></span>|<span data-ttu-id="27f8b-152">String</span><span class="sxs-lookup"><span data-stu-id="27f8b-152">String</span></span>|<span data-ttu-id="27f8b-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27f8b-153">Not yet documented</span></span>|
|<span data-ttu-id="27f8b-154">cert3PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="27f8b-154">cert3PayloadUUID</span></span>|<span data-ttu-id="27f8b-155">String</span><span class="sxs-lookup"><span data-stu-id="27f8b-155">String</span></span>|<span data-ttu-id="27f8b-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27f8b-156">Not yet documented</span></span>|
|<span data-ttu-id="27f8b-157">плисттемплате</span><span class="sxs-lookup"><span data-stu-id="27f8b-157">plistTemplate</span></span>|<span data-ttu-id="27f8b-158">String</span><span class="sxs-lookup"><span data-stu-id="27f8b-158">String</span></span>|<span data-ttu-id="27f8b-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27f8b-159">Not yet documented</span></span>|
|<span data-ttu-id="27f8b-160">енкриптедблоб</span><span class="sxs-lookup"><span data-stu-id="27f8b-160">encryptedBlob</span></span>|<span data-ttu-id="27f8b-161">Binary</span><span class="sxs-lookup"><span data-stu-id="27f8b-161">Binary</span></span>|<span data-ttu-id="27f8b-162">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27f8b-162">Not yet documented</span></span>|
|<span data-ttu-id="27f8b-163">пайлоадверсион</span><span class="sxs-lookup"><span data-stu-id="27f8b-163">payloadVersion</span></span>|<span data-ttu-id="27f8b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="27f8b-164">Int32</span></span>|<span data-ttu-id="27f8b-165">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="27f8b-165">Not yet documented</span></span>|
|<span data-ttu-id="27f8b-166">status</span><span class="sxs-lookup"><span data-stu-id="27f8b-166">status</span></span>|<span data-ttu-id="27f8b-167">Int32</span><span class="sxs-lookup"><span data-stu-id="27f8b-167">Int32</span></span>|<span data-ttu-id="27f8b-168">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="27f8b-168">Not yet documented</span></span>|
|<span data-ttu-id="27f8b-169">createdTime</span><span class="sxs-lookup"><span data-stu-id="27f8b-169">createdTime</span></span>|<span data-ttu-id="27f8b-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27f8b-170">DateTimeOffset</span></span>|<span data-ttu-id="27f8b-171">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27f8b-171">Not yet documented</span></span>|
|<span data-ttu-id="27f8b-172">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="27f8b-172">lastModifiedTime</span></span>|<span data-ttu-id="27f8b-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27f8b-173">DateTimeOffset</span></span>|<span data-ttu-id="27f8b-174">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27f8b-174">Not yet documented</span></span>|
|<span data-ttu-id="27f8b-175">eTag</span><span class="sxs-lookup"><span data-stu-id="27f8b-175">eTag</span></span>|<span data-ttu-id="27f8b-176">String</span><span class="sxs-lookup"><span data-stu-id="27f8b-176">String</span></span>|<span data-ttu-id="27f8b-177">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27f8b-177">Not yet documented</span></span>|
|<span data-ttu-id="27f8b-178">isDeleted</span><span class="sxs-lookup"><span data-stu-id="27f8b-178">isDeleted</span></span>|<span data-ttu-id="27f8b-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="27f8b-179">Boolean</span></span>|<span data-ttu-id="27f8b-180">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27f8b-180">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="27f8b-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="27f8b-181">Response</span></span>
<span data-ttu-id="27f8b-182">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="27f8b-182">If successful, this method returns a `201 Created` response code and a [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27f8b-183">Пример</span><span class="sxs-lookup"><span data-stu-id="27f8b-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="27f8b-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="27f8b-184">Request</span></span>
<span data-ttu-id="27f8b-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27f8b-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="27f8b-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="27f8b-186">Response</span></span>
<span data-ttu-id="27f8b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27f8b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





