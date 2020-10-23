---
title: Обновление Онпременкриптедпайлоад
description: Обновление свойств объекта Онпременкриптедпайлоад.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 16bc722d914c961615962061870fe7c41ea00340
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706417"
---
# <a name="update-onpremencryptedpayload"></a><span data-ttu-id="9cfac-103">Обновление Онпременкриптедпайлоад</span><span class="sxs-lookup"><span data-stu-id="9cfac-103">Update onPremEncryptedPayload</span></span>

<span data-ttu-id="9cfac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cfac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9cfac-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cfac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cfac-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9cfac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cfac-107">Обновление свойств объекта [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) .</span><span class="sxs-lookup"><span data-stu-id="9cfac-107">Update the properties of a [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9cfac-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9cfac-108">Prerequisites</span></span>
<span data-ttu-id="9cfac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cfac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cfac-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9cfac-111">Permission type</span></span>|<span data-ttu-id="9cfac-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9cfac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cfac-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9cfac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9cfac-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cfac-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9cfac-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9cfac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cfac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cfac-116">Not supported.</span></span>|
|<span data-ttu-id="9cfac-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9cfac-117">Application</span></span>|<span data-ttu-id="9cfac-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cfac-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cfac-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9cfac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
```

## <a name="request-headers"></a><span data-ttu-id="9cfac-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9cfac-120">Request headers</span></span>
|<span data-ttu-id="9cfac-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9cfac-121">Header</span></span>|<span data-ttu-id="9cfac-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9cfac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cfac-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9cfac-123">Authorization</span></span>|<span data-ttu-id="9cfac-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9cfac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cfac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9cfac-125">Accept</span></span>|<span data-ttu-id="9cfac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9cfac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cfac-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9cfac-127">Request body</span></span>
<span data-ttu-id="9cfac-128">В тексте запроса добавьте представление объекта [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9cfac-128">In the request body, supply a JSON representation for the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

<span data-ttu-id="9cfac-129">В следующей таблице приведены свойства, необходимые при создании [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md).</span><span class="sxs-lookup"><span data-stu-id="9cfac-129">The following table shows the properties that are required when you create the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md).</span></span>

|<span data-ttu-id="9cfac-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9cfac-130">Property</span></span>|<span data-ttu-id="9cfac-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9cfac-131">Type</span></span>|<span data-ttu-id="9cfac-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9cfac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cfac-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="9cfac-133">tenantId</span></span>|<span data-ttu-id="9cfac-134">Guid</span><span class="sxs-lookup"><span data-stu-id="9cfac-134">Guid</span></span>|<span data-ttu-id="9cfac-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9cfac-135">Not yet documented</span></span>|
|<span data-ttu-id="9cfac-136">userId</span><span class="sxs-lookup"><span data-stu-id="9cfac-136">userId</span></span>|<span data-ttu-id="9cfac-137">Guid</span><span class="sxs-lookup"><span data-stu-id="9cfac-137">Guid</span></span>|<span data-ttu-id="9cfac-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9cfac-138">Not yet documented</span></span>|
|<span data-ttu-id="9cfac-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="9cfac-139">deviceId</span></span>|<span data-ttu-id="9cfac-140">Guid</span><span class="sxs-lookup"><span data-stu-id="9cfac-140">Guid</span></span>|<span data-ttu-id="9cfac-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9cfac-141">Not yet documented</span></span>|
|<span data-ttu-id="9cfac-142">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="9cfac-142">payloadId</span></span>|<span data-ttu-id="9cfac-143">Guid</span><span class="sxs-lookup"><span data-stu-id="9cfac-143">Guid</span></span>|<span data-ttu-id="9cfac-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9cfac-144">Not yet documented</span></span>|
|<span data-ttu-id="9cfac-145">девицекэйсумбпринт</span><span class="sxs-lookup"><span data-stu-id="9cfac-145">deviceKeyThumbprint</span></span>|<span data-ttu-id="9cfac-146">String</span><span class="sxs-lookup"><span data-stu-id="9cfac-146">String</span></span>|<span data-ttu-id="9cfac-147">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9cfac-147">Not yet documented</span></span>|
|<span data-ttu-id="9cfac-148">cert1PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="9cfac-148">cert1PayloadUUID</span></span>|<span data-ttu-id="9cfac-149">String</span><span class="sxs-lookup"><span data-stu-id="9cfac-149">String</span></span>|<span data-ttu-id="9cfac-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9cfac-150">Not yet documented</span></span>|
|<span data-ttu-id="9cfac-151">cert2PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="9cfac-151">cert2PayloadUUID</span></span>|<span data-ttu-id="9cfac-152">String</span><span class="sxs-lookup"><span data-stu-id="9cfac-152">String</span></span>|<span data-ttu-id="9cfac-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9cfac-153">Not yet documented</span></span>|
|<span data-ttu-id="9cfac-154">cert3PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="9cfac-154">cert3PayloadUUID</span></span>|<span data-ttu-id="9cfac-155">String</span><span class="sxs-lookup"><span data-stu-id="9cfac-155">String</span></span>|<span data-ttu-id="9cfac-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9cfac-156">Not yet documented</span></span>|
|<span data-ttu-id="9cfac-157">плисттемплате</span><span class="sxs-lookup"><span data-stu-id="9cfac-157">plistTemplate</span></span>|<span data-ttu-id="9cfac-158">String</span><span class="sxs-lookup"><span data-stu-id="9cfac-158">String</span></span>|<span data-ttu-id="9cfac-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9cfac-159">Not yet documented</span></span>|
|<span data-ttu-id="9cfac-160">енкриптедблоб</span><span class="sxs-lookup"><span data-stu-id="9cfac-160">encryptedBlob</span></span>|<span data-ttu-id="9cfac-161">Binary</span><span class="sxs-lookup"><span data-stu-id="9cfac-161">Binary</span></span>|<span data-ttu-id="9cfac-162">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9cfac-162">Not yet documented</span></span>|
|<span data-ttu-id="9cfac-163">пайлоадверсион</span><span class="sxs-lookup"><span data-stu-id="9cfac-163">payloadVersion</span></span>|<span data-ttu-id="9cfac-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9cfac-164">Int32</span></span>|<span data-ttu-id="9cfac-165">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9cfac-165">Not yet documented</span></span>|
|<span data-ttu-id="9cfac-166">status</span><span class="sxs-lookup"><span data-stu-id="9cfac-166">status</span></span>|<span data-ttu-id="9cfac-167">Int32</span><span class="sxs-lookup"><span data-stu-id="9cfac-167">Int32</span></span>|<span data-ttu-id="9cfac-168">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9cfac-168">Not yet documented</span></span>|
|<span data-ttu-id="9cfac-169">createdTime</span><span class="sxs-lookup"><span data-stu-id="9cfac-169">createdTime</span></span>|<span data-ttu-id="9cfac-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cfac-170">DateTimeOffset</span></span>|<span data-ttu-id="9cfac-171">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9cfac-171">Not yet documented</span></span>|
|<span data-ttu-id="9cfac-172">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="9cfac-172">lastModifiedTime</span></span>|<span data-ttu-id="9cfac-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cfac-173">DateTimeOffset</span></span>|<span data-ttu-id="9cfac-174">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9cfac-174">Not yet documented</span></span>|
|<span data-ttu-id="9cfac-175">eTag</span><span class="sxs-lookup"><span data-stu-id="9cfac-175">eTag</span></span>|<span data-ttu-id="9cfac-176">String</span><span class="sxs-lookup"><span data-stu-id="9cfac-176">String</span></span>|<span data-ttu-id="9cfac-177">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9cfac-177">Not yet documented</span></span>|
|<span data-ttu-id="9cfac-178">isDeleted</span><span class="sxs-lookup"><span data-stu-id="9cfac-178">isDeleted</span></span>|<span data-ttu-id="9cfac-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cfac-179">Boolean</span></span>|<span data-ttu-id="9cfac-180">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9cfac-180">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9cfac-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="9cfac-181">Response</span></span>
<span data-ttu-id="9cfac-182">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9cfac-182">If successful, this method returns a `200 OK` response code and an updated [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cfac-183">Пример</span><span class="sxs-lookup"><span data-stu-id="9cfac-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="9cfac-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="9cfac-184">Request</span></span>
<span data-ttu-id="9cfac-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9cfac-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
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

### <a name="response"></a><span data-ttu-id="9cfac-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cfac-186">Response</span></span>
<span data-ttu-id="9cfac-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9cfac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





