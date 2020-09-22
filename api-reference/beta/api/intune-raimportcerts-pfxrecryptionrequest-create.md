---
title: Создание Пфксрекриптионрекуест
description: Создание нового объекта Пфксрекриптионрекуест.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0b961e11bf5ee6fc34e8e9d9fe9e70e5b0f3dd7b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093247"
---
# <a name="create-pfxrecryptionrequest"></a><span data-ttu-id="5d0c5-103">Создание Пфксрекриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="5d0c5-103">Create pfxRecryptionRequest</span></span>

<span data-ttu-id="5d0c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d0c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d0c5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d0c5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d0c5-107">Создание нового объекта [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="5d0c5-107">Create a new [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d0c5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5d0c5-108">Prerequisites</span></span>
<span data-ttu-id="5d0c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d0c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d0c5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d0c5-111">Permission type</span></span>|<span data-ttu-id="5d0c5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d0c5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d0c5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d0c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5d0c5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d0c5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5d0c5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d0c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d0c5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-116">Not supported.</span></span>|
|<span data-ttu-id="5d0c5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d0c5-117">Application</span></span>|<span data-ttu-id="5d0c5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d0c5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d0c5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d0c5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxRecryptionRequests
```

## <a name="request-headers"></a><span data-ttu-id="5d0c5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5d0c5-120">Request headers</span></span>
|<span data-ttu-id="5d0c5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5d0c5-121">Header</span></span>|<span data-ttu-id="5d0c5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5d0c5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d0c5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d0c5-123">Authorization</span></span>|<span data-ttu-id="5d0c5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d0c5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5d0c5-125">Accept</span></span>|<span data-ttu-id="5d0c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5d0c5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d0c5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d0c5-127">Request body</span></span>
<span data-ttu-id="5d0c5-128">В тексте запроса добавьте представление объекта Пфксрекриптионрекуест в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-128">In the request body, supply a JSON representation for the pfxRecryptionRequest object.</span></span>

<span data-ttu-id="5d0c5-129">В следующей таблице приведены свойства, необходимые при создании Пфксрекриптионрекуест.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-129">The following table shows the properties that are required when you create the pfxRecryptionRequest.</span></span>

|<span data-ttu-id="5d0c5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d0c5-130">Property</span></span>|<span data-ttu-id="5d0c5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5d0c5-131">Type</span></span>|<span data-ttu-id="5d0c5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5d0c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d0c5-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="5d0c5-133">tenantId</span></span>|<span data-ttu-id="5d0c5-134">Guid</span><span class="sxs-lookup"><span data-stu-id="5d0c5-134">Guid</span></span>|<span data-ttu-id="5d0c5-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-135">Not yet documented</span></span>|
|<span data-ttu-id="5d0c5-136">userId</span><span class="sxs-lookup"><span data-stu-id="5d0c5-136">userId</span></span>|<span data-ttu-id="5d0c5-137">Guid</span><span class="sxs-lookup"><span data-stu-id="5d0c5-137">Guid</span></span>|<span data-ttu-id="5d0c5-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-138">Not yet documented</span></span>|
|<span data-ttu-id="5d0c5-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="5d0c5-139">deviceId</span></span>|<span data-ttu-id="5d0c5-140">Guid</span><span class="sxs-lookup"><span data-stu-id="5d0c5-140">Guid</span></span>|<span data-ttu-id="5d0c5-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-141">Not yet documented</span></span>|
|<span data-ttu-id="5d0c5-142">профилеид</span><span class="sxs-lookup"><span data-stu-id="5d0c5-142">profileId</span></span>|<span data-ttu-id="5d0c5-143">Guid</span><span class="sxs-lookup"><span data-stu-id="5d0c5-143">Guid</span></span>|<span data-ttu-id="5d0c5-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-144">Not yet documented</span></span>|
|<span data-ttu-id="5d0c5-145">отпечаток</span><span class="sxs-lookup"><span data-stu-id="5d0c5-145">thumbprint</span></span>|<span data-ttu-id="5d0c5-146">String</span><span class="sxs-lookup"><span data-stu-id="5d0c5-146">String</span></span>|<span data-ttu-id="5d0c5-147">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-147">Not yet documented</span></span>|
|<span data-ttu-id="5d0c5-148">девицекэйсумбпринт</span><span class="sxs-lookup"><span data-stu-id="5d0c5-148">deviceKeyThumbprint</span></span>|<span data-ttu-id="5d0c5-149">String</span><span class="sxs-lookup"><span data-stu-id="5d0c5-149">String</span></span>|<span data-ttu-id="5d0c5-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-150">Not yet documented</span></span>|
|<span data-ttu-id="5d0c5-151">status</span><span class="sxs-lookup"><span data-stu-id="5d0c5-151">status</span></span>|<span data-ttu-id="5d0c5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5d0c5-152">Int32</span></span>|<span data-ttu-id="5d0c5-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-153">Not yet documented</span></span>|
|<span data-ttu-id="5d0c5-154">sourceType</span><span class="sxs-lookup"><span data-stu-id="5d0c5-154">sourceType</span></span>|<span data-ttu-id="5d0c5-155">Int32</span><span class="sxs-lookup"><span data-stu-id="5d0c5-155">Int32</span></span>|<span data-ttu-id="5d0c5-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-156">Not yet documented</span></span>|
|<span data-ttu-id="5d0c5-157">createdTime</span><span class="sxs-lookup"><span data-stu-id="5d0c5-157">createdTime</span></span>|<span data-ttu-id="5d0c5-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d0c5-158">DateTimeOffset</span></span>|<span data-ttu-id="5d0c5-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-159">Not yet documented</span></span>|
|<span data-ttu-id="5d0c5-160">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="5d0c5-160">lastModifiedTime</span></span>|<span data-ttu-id="5d0c5-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d0c5-161">DateTimeOffset</span></span>|<span data-ttu-id="5d0c5-162">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-162">Not yet documented</span></span>|
|<span data-ttu-id="5d0c5-163">isDeleted</span><span class="sxs-lookup"><span data-stu-id="5d0c5-163">isDeleted</span></span>|<span data-ttu-id="5d0c5-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d0c5-164">Boolean</span></span>|<span data-ttu-id="5d0c5-165">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5d0c5-165">Not yet documented</span></span>|
|<span data-ttu-id="5d0c5-166">eTag</span><span class="sxs-lookup"><span data-stu-id="5d0c5-166">eTag</span></span>|<span data-ttu-id="5d0c5-167">String</span><span class="sxs-lookup"><span data-stu-id="5d0c5-167">String</span></span>|<span data-ttu-id="5d0c5-168">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-168">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5d0c5-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="5d0c5-169">Response</span></span>
<span data-ttu-id="5d0c5-170">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-170">If successful, this method returns a `201 Created` response code and a [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d0c5-171">Пример</span><span class="sxs-lookup"><span data-stu-id="5d0c5-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d0c5-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d0c5-172">Request</span></span>
<span data-ttu-id="5d0c5-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/pfxRecryptionRequests
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

### <a name="response"></a><span data-ttu-id="5d0c5-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d0c5-174">Response</span></span>
<span data-ttu-id="5d0c5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






