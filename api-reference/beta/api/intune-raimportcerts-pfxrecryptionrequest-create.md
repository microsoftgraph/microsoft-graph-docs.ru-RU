---
title: Создание Пфксрекриптионрекуест
description: Создание нового объекта Пфксрекриптионрекуест.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: da46e7525c2dcf2b8ab86eb1a71108fc4577424c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460138"
---
# <a name="create-pfxrecryptionrequest"></a><span data-ttu-id="08397-103">Создание Пфксрекриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="08397-103">Create pfxRecryptionRequest</span></span>

<span data-ttu-id="08397-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="08397-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08397-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08397-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08397-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08397-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08397-107">Создание нового объекта [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="08397-107">Create a new [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08397-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="08397-108">Prerequisites</span></span>
<span data-ttu-id="08397-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08397-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08397-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08397-111">Permission type</span></span>|<span data-ttu-id="08397-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08397-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08397-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08397-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08397-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08397-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08397-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08397-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08397-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08397-116">Not supported.</span></span>|
|<span data-ttu-id="08397-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08397-117">Application</span></span>|<span data-ttu-id="08397-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08397-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08397-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08397-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxRecryptionRequests
```

## <a name="request-headers"></a><span data-ttu-id="08397-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="08397-120">Request headers</span></span>
|<span data-ttu-id="08397-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08397-121">Header</span></span>|<span data-ttu-id="08397-122">Значение</span><span class="sxs-lookup"><span data-stu-id="08397-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08397-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08397-123">Authorization</span></span>|<span data-ttu-id="08397-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08397-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08397-125">Accept</span><span class="sxs-lookup"><span data-stu-id="08397-125">Accept</span></span>|<span data-ttu-id="08397-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08397-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08397-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08397-127">Request body</span></span>
<span data-ttu-id="08397-128">В тексте запроса добавьте представление объекта Пфксрекриптионрекуест в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08397-128">In the request body, supply a JSON representation for the pfxRecryptionRequest object.</span></span>

<span data-ttu-id="08397-129">В следующей таблице приведены свойства, необходимые при создании Пфксрекриптионрекуест.</span><span class="sxs-lookup"><span data-stu-id="08397-129">The following table shows the properties that are required when you create the pfxRecryptionRequest.</span></span>

|<span data-ttu-id="08397-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="08397-130">Property</span></span>|<span data-ttu-id="08397-131">Тип</span><span class="sxs-lookup"><span data-stu-id="08397-131">Type</span></span>|<span data-ttu-id="08397-132">Описание</span><span class="sxs-lookup"><span data-stu-id="08397-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08397-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="08397-133">tenantId</span></span>|<span data-ttu-id="08397-134">GUID</span><span class="sxs-lookup"><span data-stu-id="08397-134">Guid</span></span>|<span data-ttu-id="08397-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="08397-135">Not yet documented</span></span>|
|<span data-ttu-id="08397-136">userId</span><span class="sxs-lookup"><span data-stu-id="08397-136">userId</span></span>|<span data-ttu-id="08397-137">GUID</span><span class="sxs-lookup"><span data-stu-id="08397-137">Guid</span></span>|<span data-ttu-id="08397-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="08397-138">Not yet documented</span></span>|
|<span data-ttu-id="08397-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="08397-139">deviceId</span></span>|<span data-ttu-id="08397-140">Guid</span><span class="sxs-lookup"><span data-stu-id="08397-140">Guid</span></span>|<span data-ttu-id="08397-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="08397-141">Not yet documented</span></span>|
|<span data-ttu-id="08397-142">профилеид</span><span class="sxs-lookup"><span data-stu-id="08397-142">profileId</span></span>|<span data-ttu-id="08397-143">GUID</span><span class="sxs-lookup"><span data-stu-id="08397-143">Guid</span></span>|<span data-ttu-id="08397-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="08397-144">Not yet documented</span></span>|
|<span data-ttu-id="08397-145">отпечаток</span><span class="sxs-lookup"><span data-stu-id="08397-145">thumbprint</span></span>|<span data-ttu-id="08397-146">String</span><span class="sxs-lookup"><span data-stu-id="08397-146">String</span></span>|<span data-ttu-id="08397-147">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="08397-147">Not yet documented</span></span>|
|<span data-ttu-id="08397-148">девицекэйсумбпринт</span><span class="sxs-lookup"><span data-stu-id="08397-148">deviceKeyThumbprint</span></span>|<span data-ttu-id="08397-149">String</span><span class="sxs-lookup"><span data-stu-id="08397-149">String</span></span>|<span data-ttu-id="08397-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="08397-150">Not yet documented</span></span>|
|<span data-ttu-id="08397-151">status</span><span class="sxs-lookup"><span data-stu-id="08397-151">status</span></span>|<span data-ttu-id="08397-152">Int32</span><span class="sxs-lookup"><span data-stu-id="08397-152">Int32</span></span>|<span data-ttu-id="08397-153">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="08397-153">Not yet documented</span></span>|
|<span data-ttu-id="08397-154">sourceType</span><span class="sxs-lookup"><span data-stu-id="08397-154">sourceType</span></span>|<span data-ttu-id="08397-155">Int32</span><span class="sxs-lookup"><span data-stu-id="08397-155">Int32</span></span>|<span data-ttu-id="08397-156">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="08397-156">Not yet documented</span></span>|
|<span data-ttu-id="08397-157">createdTime</span><span class="sxs-lookup"><span data-stu-id="08397-157">createdTime</span></span>|<span data-ttu-id="08397-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08397-158">DateTimeOffset</span></span>|<span data-ttu-id="08397-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="08397-159">Not yet documented</span></span>|
|<span data-ttu-id="08397-160">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="08397-160">lastModifiedTime</span></span>|<span data-ttu-id="08397-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08397-161">DateTimeOffset</span></span>|<span data-ttu-id="08397-162">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="08397-162">Not yet documented</span></span>|
|<span data-ttu-id="08397-163">isDeleted</span><span class="sxs-lookup"><span data-stu-id="08397-163">isDeleted</span></span>|<span data-ttu-id="08397-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="08397-164">Boolean</span></span>|<span data-ttu-id="08397-165">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="08397-165">Not yet documented</span></span>|
|<span data-ttu-id="08397-166">eTag</span><span class="sxs-lookup"><span data-stu-id="08397-166">eTag</span></span>|<span data-ttu-id="08397-167">String</span><span class="sxs-lookup"><span data-stu-id="08397-167">String</span></span>|<span data-ttu-id="08397-168">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="08397-168">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="08397-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="08397-169">Response</span></span>
<span data-ttu-id="08397-170">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08397-170">If successful, this method returns a `201 Created` response code and a [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08397-171">Пример</span><span class="sxs-lookup"><span data-stu-id="08397-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="08397-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="08397-172">Request</span></span>
<span data-ttu-id="08397-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08397-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="08397-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="08397-174">Response</span></span>
<span data-ttu-id="08397-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08397-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





