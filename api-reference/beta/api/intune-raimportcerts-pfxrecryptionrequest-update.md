---
title: Обновление Пфксрекриптионрекуест
description: Обновление свойств объекта Пфксрекриптионрекуест.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2170ea824102db4e564dee5bc210852a30739aae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093184"
---
# <a name="update-pfxrecryptionrequest"></a><span data-ttu-id="8c51d-103">Обновление Пфксрекриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="8c51d-103">Update pfxRecryptionRequest</span></span>

<span data-ttu-id="8c51d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c51d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c51d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c51d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c51d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c51d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c51d-107">Обновление свойств объекта [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="8c51d-107">Update the properties of a [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c51d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8c51d-108">Prerequisites</span></span>
<span data-ttu-id="8c51d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c51d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c51d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c51d-111">Permission type</span></span>|<span data-ttu-id="8c51d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c51d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c51d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c51d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c51d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c51d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8c51d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c51d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c51d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c51d-116">Not supported.</span></span>|
|<span data-ttu-id="8c51d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c51d-117">Application</span></span>|<span data-ttu-id="8c51d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c51d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c51d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c51d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxRecryptionRequests/{pfxRecryptionRequestsId}
```

## <a name="request-headers"></a><span data-ttu-id="8c51d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8c51d-120">Request headers</span></span>
|<span data-ttu-id="8c51d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c51d-121">Header</span></span>|<span data-ttu-id="8c51d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8c51d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c51d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c51d-123">Authorization</span></span>|<span data-ttu-id="8c51d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c51d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c51d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8c51d-125">Accept</span></span>|<span data-ttu-id="8c51d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c51d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c51d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c51d-127">Request body</span></span>
<span data-ttu-id="8c51d-128">В тексте запроса добавьте представление объекта [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c51d-128">In the request body, supply a JSON representation for the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

<span data-ttu-id="8c51d-129">В следующей таблице приведены свойства, необходимые при создании [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md).</span><span class="sxs-lookup"><span data-stu-id="8c51d-129">The following table shows the properties that are required when you create the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md).</span></span>

|<span data-ttu-id="8c51d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c51d-130">Property</span></span>|<span data-ttu-id="8c51d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8c51d-131">Type</span></span>|<span data-ttu-id="8c51d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8c51d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c51d-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="8c51d-133">tenantId</span></span>|<span data-ttu-id="8c51d-134">Guid</span><span class="sxs-lookup"><span data-stu-id="8c51d-134">Guid</span></span>|<span data-ttu-id="8c51d-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c51d-135">Not yet documented</span></span>|
|<span data-ttu-id="8c51d-136">userId</span><span class="sxs-lookup"><span data-stu-id="8c51d-136">userId</span></span>|<span data-ttu-id="8c51d-137">Guid</span><span class="sxs-lookup"><span data-stu-id="8c51d-137">Guid</span></span>|<span data-ttu-id="8c51d-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c51d-138">Not yet documented</span></span>|
|<span data-ttu-id="8c51d-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="8c51d-139">deviceId</span></span>|<span data-ttu-id="8c51d-140">Guid</span><span class="sxs-lookup"><span data-stu-id="8c51d-140">Guid</span></span>|<span data-ttu-id="8c51d-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c51d-141">Not yet documented</span></span>|
|<span data-ttu-id="8c51d-142">профилеид</span><span class="sxs-lookup"><span data-stu-id="8c51d-142">profileId</span></span>|<span data-ttu-id="8c51d-143">Guid</span><span class="sxs-lookup"><span data-stu-id="8c51d-143">Guid</span></span>|<span data-ttu-id="8c51d-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c51d-144">Not yet documented</span></span>|
|<span data-ttu-id="8c51d-145">отпечаток</span><span class="sxs-lookup"><span data-stu-id="8c51d-145">thumbprint</span></span>|<span data-ttu-id="8c51d-146">String</span><span class="sxs-lookup"><span data-stu-id="8c51d-146">String</span></span>|<span data-ttu-id="8c51d-147">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c51d-147">Not yet documented</span></span>|
|<span data-ttu-id="8c51d-148">девицекэйсумбпринт</span><span class="sxs-lookup"><span data-stu-id="8c51d-148">deviceKeyThumbprint</span></span>|<span data-ttu-id="8c51d-149">String</span><span class="sxs-lookup"><span data-stu-id="8c51d-149">String</span></span>|<span data-ttu-id="8c51d-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c51d-150">Not yet documented</span></span>|
|<span data-ttu-id="8c51d-151">status</span><span class="sxs-lookup"><span data-stu-id="8c51d-151">status</span></span>|<span data-ttu-id="8c51d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8c51d-152">Int32</span></span>|<span data-ttu-id="8c51d-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c51d-153">Not yet documented</span></span>|
|<span data-ttu-id="8c51d-154">sourceType</span><span class="sxs-lookup"><span data-stu-id="8c51d-154">sourceType</span></span>|<span data-ttu-id="8c51d-155">Int32</span><span class="sxs-lookup"><span data-stu-id="8c51d-155">Int32</span></span>|<span data-ttu-id="8c51d-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c51d-156">Not yet documented</span></span>|
|<span data-ttu-id="8c51d-157">createdTime</span><span class="sxs-lookup"><span data-stu-id="8c51d-157">createdTime</span></span>|<span data-ttu-id="8c51d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c51d-158">DateTimeOffset</span></span>|<span data-ttu-id="8c51d-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c51d-159">Not yet documented</span></span>|
|<span data-ttu-id="8c51d-160">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="8c51d-160">lastModifiedTime</span></span>|<span data-ttu-id="8c51d-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c51d-161">DateTimeOffset</span></span>|<span data-ttu-id="8c51d-162">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c51d-162">Not yet documented</span></span>|
|<span data-ttu-id="8c51d-163">isDeleted</span><span class="sxs-lookup"><span data-stu-id="8c51d-163">isDeleted</span></span>|<span data-ttu-id="8c51d-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c51d-164">Boolean</span></span>|<span data-ttu-id="8c51d-165">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8c51d-165">Not yet documented</span></span>|
|<span data-ttu-id="8c51d-166">eTag</span><span class="sxs-lookup"><span data-stu-id="8c51d-166">eTag</span></span>|<span data-ttu-id="8c51d-167">String</span><span class="sxs-lookup"><span data-stu-id="8c51d-167">String</span></span>|<span data-ttu-id="8c51d-168">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c51d-168">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8c51d-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c51d-169">Response</span></span>
<span data-ttu-id="8c51d-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c51d-170">If successful, this method returns a `200 OK` response code and an updated [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c51d-171">Пример</span><span class="sxs-lookup"><span data-stu-id="8c51d-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c51d-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c51d-172">Request</span></span>
<span data-ttu-id="8c51d-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c51d-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/pfxRecryptionRequests/{pfxRecryptionRequestsId}
Content-type: application/json
Content-length: 574

{
  "@odata.type": "#microsoft.graph.pfxRecryptionRequest",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
  "profileId": "6389d896-d896-6389-96d8-896396d88963",
  "thumbprint": "Thumbprint value",
  "deviceKeyThumbprint": "Device Key Thumbprint value",
  "status": 6,
  "sourceType": 10,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "isDeleted": true,
  "eTag": "ETag value"
}
```

### <a name="response"></a><span data-ttu-id="8c51d-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c51d-174">Response</span></span>
<span data-ttu-id="8c51d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c51d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.pfxRecryptionRequest",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
  "profileId": "6389d896-d896-6389-96d8-896396d88963",
  "thumbprint": "Thumbprint value",
  "deviceKeyThumbprint": "Device Key Thumbprint value",
  "status": 6,
  "sourceType": 10,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "isDeleted": true,
  "eTag": "ETag value"
}
```






