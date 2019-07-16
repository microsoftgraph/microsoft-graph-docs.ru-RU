---
title: Обновление Онпременкриптедпайлоад
description: Обновление свойств объекта Онпременкриптедпайлоад.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a50048080072c8bcc7feb08cac69d74a18460c19
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741503"
---
# <a name="update-onpremencryptedpayload"></a><span data-ttu-id="264bd-103">Обновление Онпременкриптедпайлоад</span><span class="sxs-lookup"><span data-stu-id="264bd-103">Update onPremEncryptedPayload</span></span>

> <span data-ttu-id="264bd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="264bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="264bd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="264bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="264bd-106">Обновление свойств объекта [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) .</span><span class="sxs-lookup"><span data-stu-id="264bd-106">Update the properties of a [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="264bd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="264bd-107">Prerequisites</span></span>
<span data-ttu-id="264bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="264bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="264bd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="264bd-110">Permission type</span></span>|<span data-ttu-id="264bd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="264bd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="264bd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="264bd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="264bd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="264bd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="264bd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="264bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="264bd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="264bd-115">Not supported.</span></span>|
|<span data-ttu-id="264bd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="264bd-116">Application</span></span>|<span data-ttu-id="264bd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="264bd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="264bd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="264bd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
```

## <a name="request-headers"></a><span data-ttu-id="264bd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="264bd-119">Request headers</span></span>
|<span data-ttu-id="264bd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="264bd-120">Header</span></span>|<span data-ttu-id="264bd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="264bd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="264bd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="264bd-122">Authorization</span></span>|<span data-ttu-id="264bd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="264bd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="264bd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="264bd-124">Accept</span></span>|<span data-ttu-id="264bd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="264bd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="264bd-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="264bd-126">Request body</span></span>
<span data-ttu-id="264bd-127">В тексте запроса добавьте представление объекта [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="264bd-127">In the request body, supply a JSON representation for the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

<span data-ttu-id="264bd-128">В следующей таблице приведены свойства, необходимые при создании [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md).</span><span class="sxs-lookup"><span data-stu-id="264bd-128">The following table shows the properties that are required when you create the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md).</span></span>

|<span data-ttu-id="264bd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="264bd-129">Property</span></span>|<span data-ttu-id="264bd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="264bd-130">Type</span></span>|<span data-ttu-id="264bd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="264bd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="264bd-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="264bd-132">tenantId</span></span>|<span data-ttu-id="264bd-133">GUID</span><span class="sxs-lookup"><span data-stu-id="264bd-133">Guid</span></span>|<span data-ttu-id="264bd-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="264bd-134">Not yet documented</span></span>|
|<span data-ttu-id="264bd-135">userId</span><span class="sxs-lookup"><span data-stu-id="264bd-135">userId</span></span>|<span data-ttu-id="264bd-136">GUID</span><span class="sxs-lookup"><span data-stu-id="264bd-136">Guid</span></span>|<span data-ttu-id="264bd-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="264bd-137">Not yet documented</span></span>|
|<span data-ttu-id="264bd-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="264bd-138">deviceId</span></span>|<span data-ttu-id="264bd-139">Guid</span><span class="sxs-lookup"><span data-stu-id="264bd-139">Guid</span></span>|<span data-ttu-id="264bd-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="264bd-140">Not yet documented</span></span>|
|<span data-ttu-id="264bd-141">Пайлоадид</span><span class="sxs-lookup"><span data-stu-id="264bd-141">payloadId</span></span>|<span data-ttu-id="264bd-142">GUID</span><span class="sxs-lookup"><span data-stu-id="264bd-142">Guid</span></span>|<span data-ttu-id="264bd-143">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="264bd-143">Not yet documented</span></span>|
|<span data-ttu-id="264bd-144">Девицекэйсумбпринт</span><span class="sxs-lookup"><span data-stu-id="264bd-144">deviceKeyThumbprint</span></span>|<span data-ttu-id="264bd-145">String</span><span class="sxs-lookup"><span data-stu-id="264bd-145">String</span></span>|<span data-ttu-id="264bd-146">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="264bd-146">Not yet documented</span></span>|
|<span data-ttu-id="264bd-147">cert1PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="264bd-147">cert1PayloadUUID</span></span>|<span data-ttu-id="264bd-148">String</span><span class="sxs-lookup"><span data-stu-id="264bd-148">String</span></span>|<span data-ttu-id="264bd-149">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="264bd-149">Not yet documented</span></span>|
|<span data-ttu-id="264bd-150">cert2PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="264bd-150">cert2PayloadUUID</span></span>|<span data-ttu-id="264bd-151">String</span><span class="sxs-lookup"><span data-stu-id="264bd-151">String</span></span>|<span data-ttu-id="264bd-152">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="264bd-152">Not yet documented</span></span>|
|<span data-ttu-id="264bd-153">cert3PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="264bd-153">cert3PayloadUUID</span></span>|<span data-ttu-id="264bd-154">String</span><span class="sxs-lookup"><span data-stu-id="264bd-154">String</span></span>|<span data-ttu-id="264bd-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="264bd-155">Not yet documented</span></span>|
|<span data-ttu-id="264bd-156">Плисттемплате</span><span class="sxs-lookup"><span data-stu-id="264bd-156">plistTemplate</span></span>|<span data-ttu-id="264bd-157">String</span><span class="sxs-lookup"><span data-stu-id="264bd-157">String</span></span>|<span data-ttu-id="264bd-158">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="264bd-158">Not yet documented</span></span>|
|<span data-ttu-id="264bd-159">Енкриптедблоб</span><span class="sxs-lookup"><span data-stu-id="264bd-159">encryptedBlob</span></span>|<span data-ttu-id="264bd-160">Binary</span><span class="sxs-lookup"><span data-stu-id="264bd-160">Binary</span></span>|<span data-ttu-id="264bd-161">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="264bd-161">Not yet documented</span></span>|
|<span data-ttu-id="264bd-162">Пайлоадверсион</span><span class="sxs-lookup"><span data-stu-id="264bd-162">payloadVersion</span></span>|<span data-ttu-id="264bd-163">Int32</span><span class="sxs-lookup"><span data-stu-id="264bd-163">Int32</span></span>|<span data-ttu-id="264bd-164">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="264bd-164">Not yet documented</span></span>|
|<span data-ttu-id="264bd-165">status</span><span class="sxs-lookup"><span data-stu-id="264bd-165">status</span></span>|<span data-ttu-id="264bd-166">Int32</span><span class="sxs-lookup"><span data-stu-id="264bd-166">Int32</span></span>|<span data-ttu-id="264bd-167">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="264bd-167">Not yet documented</span></span>|
|<span data-ttu-id="264bd-168">createdTime</span><span class="sxs-lookup"><span data-stu-id="264bd-168">createdTime</span></span>|<span data-ttu-id="264bd-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="264bd-169">DateTimeOffset</span></span>|<span data-ttu-id="264bd-170">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="264bd-170">Not yet documented</span></span>|
|<span data-ttu-id="264bd-171">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="264bd-171">lastModifiedTime</span></span>|<span data-ttu-id="264bd-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="264bd-172">DateTimeOffset</span></span>|<span data-ttu-id="264bd-173">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="264bd-173">Not yet documented</span></span>|
|<span data-ttu-id="264bd-174">eTag</span><span class="sxs-lookup"><span data-stu-id="264bd-174">eTag</span></span>|<span data-ttu-id="264bd-175">String</span><span class="sxs-lookup"><span data-stu-id="264bd-175">String</span></span>|<span data-ttu-id="264bd-176">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="264bd-176">Not yet documented</span></span>|
|<span data-ttu-id="264bd-177">isDeleted</span><span class="sxs-lookup"><span data-stu-id="264bd-177">isDeleted</span></span>|<span data-ttu-id="264bd-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="264bd-178">Boolean</span></span>|<span data-ttu-id="264bd-179">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="264bd-179">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="264bd-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="264bd-180">Response</span></span>
<span data-ttu-id="264bd-181">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="264bd-181">If successful, this method returns a `200 OK` response code and an updated [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="264bd-182">Пример</span><span class="sxs-lookup"><span data-stu-id="264bd-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="264bd-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="264bd-183">Request</span></span>
<span data-ttu-id="264bd-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="264bd-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="264bd-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="264bd-185">Response</span></span>
<span data-ttu-id="264bd-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="264bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





