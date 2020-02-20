---
title: Создание Пфксрекриптионрекуест
description: Создание нового объекта Пфксрекриптионрекуест.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 54d9b48396a2848a396d08760430f0c7b6418283
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161311"
---
# <a name="create-pfxrecryptionrequest"></a><span data-ttu-id="d1608-103">Создание Пфксрекриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="d1608-103">Create pfxRecryptionRequest</span></span>

> <span data-ttu-id="d1608-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1608-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1608-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1608-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1608-106">Создание нового объекта [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="d1608-106">Create a new [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1608-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d1608-107">Prerequisites</span></span>
<span data-ttu-id="d1608-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1608-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1608-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1608-110">Permission type</span></span>|<span data-ttu-id="d1608-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1608-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1608-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1608-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d1608-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1608-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1608-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1608-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1608-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1608-115">Not supported.</span></span>|
|<span data-ttu-id="d1608-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1608-116">Application</span></span>|<span data-ttu-id="d1608-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1608-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1608-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1608-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxRecryptionRequests
```

## <a name="request-headers"></a><span data-ttu-id="d1608-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d1608-119">Request headers</span></span>
|<span data-ttu-id="d1608-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1608-120">Header</span></span>|<span data-ttu-id="d1608-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d1608-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1608-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1608-122">Authorization</span></span>|<span data-ttu-id="d1608-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1608-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1608-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d1608-124">Accept</span></span>|<span data-ttu-id="d1608-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d1608-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1608-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1608-126">Request body</span></span>
<span data-ttu-id="d1608-127">В тексте запроса добавьте представление объекта Пфксрекриптионрекуест в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1608-127">In the request body, supply a JSON representation for the pfxRecryptionRequest object.</span></span>

<span data-ttu-id="d1608-128">В следующей таблице приведены свойства, необходимые при создании Пфксрекриптионрекуест.</span><span class="sxs-lookup"><span data-stu-id="d1608-128">The following table shows the properties that are required when you create the pfxRecryptionRequest.</span></span>

|<span data-ttu-id="d1608-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1608-129">Property</span></span>|<span data-ttu-id="d1608-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d1608-130">Type</span></span>|<span data-ttu-id="d1608-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d1608-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1608-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="d1608-132">tenantId</span></span>|<span data-ttu-id="d1608-133">GUID</span><span class="sxs-lookup"><span data-stu-id="d1608-133">Guid</span></span>|<span data-ttu-id="d1608-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d1608-134">Not yet documented</span></span>|
|<span data-ttu-id="d1608-135">userId</span><span class="sxs-lookup"><span data-stu-id="d1608-135">userId</span></span>|<span data-ttu-id="d1608-136">GUID</span><span class="sxs-lookup"><span data-stu-id="d1608-136">Guid</span></span>|<span data-ttu-id="d1608-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d1608-137">Not yet documented</span></span>|
|<span data-ttu-id="d1608-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="d1608-138">deviceId</span></span>|<span data-ttu-id="d1608-139">Guid</span><span class="sxs-lookup"><span data-stu-id="d1608-139">Guid</span></span>|<span data-ttu-id="d1608-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d1608-140">Not yet documented</span></span>|
|<span data-ttu-id="d1608-141">профилеид</span><span class="sxs-lookup"><span data-stu-id="d1608-141">profileId</span></span>|<span data-ttu-id="d1608-142">GUID</span><span class="sxs-lookup"><span data-stu-id="d1608-142">Guid</span></span>|<span data-ttu-id="d1608-143">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d1608-143">Not yet documented</span></span>|
|<span data-ttu-id="d1608-144">отпечаток</span><span class="sxs-lookup"><span data-stu-id="d1608-144">thumbprint</span></span>|<span data-ttu-id="d1608-145">String</span><span class="sxs-lookup"><span data-stu-id="d1608-145">String</span></span>|<span data-ttu-id="d1608-146">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d1608-146">Not yet documented</span></span>|
|<span data-ttu-id="d1608-147">девицекэйсумбпринт</span><span class="sxs-lookup"><span data-stu-id="d1608-147">deviceKeyThumbprint</span></span>|<span data-ttu-id="d1608-148">String</span><span class="sxs-lookup"><span data-stu-id="d1608-148">String</span></span>|<span data-ttu-id="d1608-149">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d1608-149">Not yet documented</span></span>|
|<span data-ttu-id="d1608-150">status</span><span class="sxs-lookup"><span data-stu-id="d1608-150">status</span></span>|<span data-ttu-id="d1608-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d1608-151">Int32</span></span>|<span data-ttu-id="d1608-152">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="d1608-152">Not yet documented</span></span>|
|<span data-ttu-id="d1608-153">sourceType</span><span class="sxs-lookup"><span data-stu-id="d1608-153">sourceType</span></span>|<span data-ttu-id="d1608-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d1608-154">Int32</span></span>|<span data-ttu-id="d1608-155">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="d1608-155">Not yet documented</span></span>|
|<span data-ttu-id="d1608-156">createdTime</span><span class="sxs-lookup"><span data-stu-id="d1608-156">createdTime</span></span>|<span data-ttu-id="d1608-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1608-157">DateTimeOffset</span></span>|<span data-ttu-id="d1608-158">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d1608-158">Not yet documented</span></span>|
|<span data-ttu-id="d1608-159">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="d1608-159">lastModifiedTime</span></span>|<span data-ttu-id="d1608-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1608-160">DateTimeOffset</span></span>|<span data-ttu-id="d1608-161">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d1608-161">Not yet documented</span></span>|
|<span data-ttu-id="d1608-162">isDeleted</span><span class="sxs-lookup"><span data-stu-id="d1608-162">isDeleted</span></span>|<span data-ttu-id="d1608-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1608-163">Boolean</span></span>|<span data-ttu-id="d1608-164">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="d1608-164">Not yet documented</span></span>|
|<span data-ttu-id="d1608-165">eTag</span><span class="sxs-lookup"><span data-stu-id="d1608-165">eTag</span></span>|<span data-ttu-id="d1608-166">String</span><span class="sxs-lookup"><span data-stu-id="d1608-166">String</span></span>|<span data-ttu-id="d1608-167">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d1608-167">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d1608-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="d1608-168">Response</span></span>
<span data-ttu-id="d1608-169">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d1608-169">If successful, this method returns a `201 Created` response code and a [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1608-170">Пример</span><span class="sxs-lookup"><span data-stu-id="d1608-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1608-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1608-171">Request</span></span>
<span data-ttu-id="d1608-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1608-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d1608-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1608-173">Response</span></span>
<span data-ttu-id="d1608-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1608-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





