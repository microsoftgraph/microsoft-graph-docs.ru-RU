---
title: Создание Онпременкриптедпайлоад
description: Создание нового объекта Онпременкриптедпайлоад.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 18adbf8cb317817cfcc1bfe21d6613f0647eed8e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49296022"
---
# <a name="create-onpremencryptedpayload"></a><span data-ttu-id="4010c-103">Создание Онпременкриптедпайлоад</span><span class="sxs-lookup"><span data-stu-id="4010c-103">Create onPremEncryptedPayload</span></span>

<span data-ttu-id="4010c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4010c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4010c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4010c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4010c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4010c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4010c-107">Создание нового объекта [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) .</span><span class="sxs-lookup"><span data-stu-id="4010c-107">Create a new [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4010c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4010c-108">Prerequisites</span></span>
<span data-ttu-id="4010c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4010c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4010c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4010c-111">Permission type</span></span>|<span data-ttu-id="4010c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4010c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4010c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4010c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4010c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4010c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4010c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4010c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4010c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4010c-116">Not supported.</span></span>|
|<span data-ttu-id="4010c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4010c-117">Application</span></span>|<span data-ttu-id="4010c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4010c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4010c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4010c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /onPremEncryptedPayloads
```

## <a name="request-headers"></a><span data-ttu-id="4010c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4010c-120">Request headers</span></span>
|<span data-ttu-id="4010c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4010c-121">Header</span></span>|<span data-ttu-id="4010c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4010c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4010c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4010c-123">Authorization</span></span>|<span data-ttu-id="4010c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4010c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4010c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4010c-125">Accept</span></span>|<span data-ttu-id="4010c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4010c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4010c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4010c-127">Request body</span></span>
<span data-ttu-id="4010c-128">В тексте запроса добавьте представление объекта Онпременкриптедпайлоад в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4010c-128">In the request body, supply a JSON representation for the onPremEncryptedPayload object.</span></span>

<span data-ttu-id="4010c-129">В следующей таблице приведены свойства, необходимые при создании Онпременкриптедпайлоад.</span><span class="sxs-lookup"><span data-stu-id="4010c-129">The following table shows the properties that are required when you create the onPremEncryptedPayload.</span></span>

|<span data-ttu-id="4010c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4010c-130">Property</span></span>|<span data-ttu-id="4010c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4010c-131">Type</span></span>|<span data-ttu-id="4010c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4010c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4010c-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="4010c-133">tenantId</span></span>|<span data-ttu-id="4010c-134">Guid</span><span class="sxs-lookup"><span data-stu-id="4010c-134">Guid</span></span>|<span data-ttu-id="4010c-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4010c-135">Not yet documented</span></span>|
|<span data-ttu-id="4010c-136">userId</span><span class="sxs-lookup"><span data-stu-id="4010c-136">userId</span></span>|<span data-ttu-id="4010c-137">Guid</span><span class="sxs-lookup"><span data-stu-id="4010c-137">Guid</span></span>|<span data-ttu-id="4010c-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4010c-138">Not yet documented</span></span>|
|<span data-ttu-id="4010c-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="4010c-139">deviceId</span></span>|<span data-ttu-id="4010c-140">Guid</span><span class="sxs-lookup"><span data-stu-id="4010c-140">Guid</span></span>|<span data-ttu-id="4010c-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4010c-141">Not yet documented</span></span>|
|<span data-ttu-id="4010c-142">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="4010c-142">payloadId</span></span>|<span data-ttu-id="4010c-143">Guid</span><span class="sxs-lookup"><span data-stu-id="4010c-143">Guid</span></span>|<span data-ttu-id="4010c-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4010c-144">Not yet documented</span></span>|
|<span data-ttu-id="4010c-145">девицекэйсумбпринт</span><span class="sxs-lookup"><span data-stu-id="4010c-145">deviceKeyThumbprint</span></span>|<span data-ttu-id="4010c-146">String</span><span class="sxs-lookup"><span data-stu-id="4010c-146">String</span></span>|<span data-ttu-id="4010c-147">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4010c-147">Not yet documented</span></span>|
|<span data-ttu-id="4010c-148">cert1PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="4010c-148">cert1PayloadUUID</span></span>|<span data-ttu-id="4010c-149">String</span><span class="sxs-lookup"><span data-stu-id="4010c-149">String</span></span>|<span data-ttu-id="4010c-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4010c-150">Not yet documented</span></span>|
|<span data-ttu-id="4010c-151">cert2PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="4010c-151">cert2PayloadUUID</span></span>|<span data-ttu-id="4010c-152">String</span><span class="sxs-lookup"><span data-stu-id="4010c-152">String</span></span>|<span data-ttu-id="4010c-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4010c-153">Not yet documented</span></span>|
|<span data-ttu-id="4010c-154">cert3PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="4010c-154">cert3PayloadUUID</span></span>|<span data-ttu-id="4010c-155">String</span><span class="sxs-lookup"><span data-stu-id="4010c-155">String</span></span>|<span data-ttu-id="4010c-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4010c-156">Not yet documented</span></span>|
|<span data-ttu-id="4010c-157">плисттемплате</span><span class="sxs-lookup"><span data-stu-id="4010c-157">plistTemplate</span></span>|<span data-ttu-id="4010c-158">String</span><span class="sxs-lookup"><span data-stu-id="4010c-158">String</span></span>|<span data-ttu-id="4010c-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4010c-159">Not yet documented</span></span>|
|<span data-ttu-id="4010c-160">енкриптедблоб</span><span class="sxs-lookup"><span data-stu-id="4010c-160">encryptedBlob</span></span>|<span data-ttu-id="4010c-161">Binary</span><span class="sxs-lookup"><span data-stu-id="4010c-161">Binary</span></span>|<span data-ttu-id="4010c-162">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4010c-162">Not yet documented</span></span>|
|<span data-ttu-id="4010c-163">пайлоадверсион</span><span class="sxs-lookup"><span data-stu-id="4010c-163">payloadVersion</span></span>|<span data-ttu-id="4010c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4010c-164">Int32</span></span>|<span data-ttu-id="4010c-165">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4010c-165">Not yet documented</span></span>|
|<span data-ttu-id="4010c-166">status</span><span class="sxs-lookup"><span data-stu-id="4010c-166">status</span></span>|<span data-ttu-id="4010c-167">Int32</span><span class="sxs-lookup"><span data-stu-id="4010c-167">Int32</span></span>|<span data-ttu-id="4010c-168">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4010c-168">Not yet documented</span></span>|
|<span data-ttu-id="4010c-169">createdTime</span><span class="sxs-lookup"><span data-stu-id="4010c-169">createdTime</span></span>|<span data-ttu-id="4010c-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4010c-170">DateTimeOffset</span></span>|<span data-ttu-id="4010c-171">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4010c-171">Not yet documented</span></span>|
|<span data-ttu-id="4010c-172">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="4010c-172">lastModifiedTime</span></span>|<span data-ttu-id="4010c-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4010c-173">DateTimeOffset</span></span>|<span data-ttu-id="4010c-174">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4010c-174">Not yet documented</span></span>|
|<span data-ttu-id="4010c-175">eTag</span><span class="sxs-lookup"><span data-stu-id="4010c-175">eTag</span></span>|<span data-ttu-id="4010c-176">String</span><span class="sxs-lookup"><span data-stu-id="4010c-176">String</span></span>|<span data-ttu-id="4010c-177">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4010c-177">Not yet documented</span></span>|
|<span data-ttu-id="4010c-178">isDeleted</span><span class="sxs-lookup"><span data-stu-id="4010c-178">isDeleted</span></span>|<span data-ttu-id="4010c-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="4010c-179">Boolean</span></span>|<span data-ttu-id="4010c-180">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4010c-180">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4010c-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="4010c-181">Response</span></span>
<span data-ttu-id="4010c-182">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4010c-182">If successful, this method returns a `201 Created` response code and a [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4010c-183">Пример</span><span class="sxs-lookup"><span data-stu-id="4010c-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="4010c-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="4010c-184">Request</span></span>
<span data-ttu-id="4010c-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4010c-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4010c-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="4010c-186">Response</span></span>
<span data-ttu-id="4010c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4010c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




