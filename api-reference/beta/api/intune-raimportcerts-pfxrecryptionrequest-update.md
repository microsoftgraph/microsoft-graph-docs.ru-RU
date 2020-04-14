---
title: Обновление Пфксрекриптионрекуест
description: Обновление свойств объекта Пфксрекриптионрекуест.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 27d5284824d561afa0e43cae570d0190e1d0e9c1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437734"
---
# <a name="update-pfxrecryptionrequest"></a><span data-ttu-id="5b184-103">Обновление Пфксрекриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="5b184-103">Update pfxRecryptionRequest</span></span>

<span data-ttu-id="5b184-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b184-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b184-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b184-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b184-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b184-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b184-107">Обновление свойств объекта [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="5b184-107">Update the properties of a [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b184-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5b184-108">Prerequisites</span></span>
<span data-ttu-id="5b184-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b184-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b184-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b184-111">Permission type</span></span>|<span data-ttu-id="5b184-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b184-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b184-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b184-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b184-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b184-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5b184-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b184-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b184-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b184-116">Not supported.</span></span>|
|<span data-ttu-id="5b184-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5b184-117">Application</span></span>|<span data-ttu-id="5b184-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b184-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b184-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b184-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxRecryptionRequests/{pfxRecryptionRequestsId}
```

## <a name="request-headers"></a><span data-ttu-id="5b184-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5b184-120">Request headers</span></span>
|<span data-ttu-id="5b184-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b184-121">Header</span></span>|<span data-ttu-id="5b184-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5b184-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b184-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b184-123">Authorization</span></span>|<span data-ttu-id="5b184-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b184-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b184-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5b184-125">Accept</span></span>|<span data-ttu-id="5b184-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b184-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b184-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b184-127">Request body</span></span>
<span data-ttu-id="5b184-128">В тексте запроса добавьте представление объекта [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b184-128">In the request body, supply a JSON representation for the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

<span data-ttu-id="5b184-129">В следующей таблице приведены свойства, необходимые при создании [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md).</span><span class="sxs-lookup"><span data-stu-id="5b184-129">The following table shows the properties that are required when you create the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md).</span></span>

|<span data-ttu-id="5b184-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b184-130">Property</span></span>|<span data-ttu-id="5b184-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5b184-131">Type</span></span>|<span data-ttu-id="5b184-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5b184-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b184-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="5b184-133">tenantId</span></span>|<span data-ttu-id="5b184-134">GUID</span><span class="sxs-lookup"><span data-stu-id="5b184-134">Guid</span></span>|<span data-ttu-id="5b184-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5b184-135">Not yet documented</span></span>|
|<span data-ttu-id="5b184-136">userId</span><span class="sxs-lookup"><span data-stu-id="5b184-136">userId</span></span>|<span data-ttu-id="5b184-137">GUID</span><span class="sxs-lookup"><span data-stu-id="5b184-137">Guid</span></span>|<span data-ttu-id="5b184-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5b184-138">Not yet documented</span></span>|
|<span data-ttu-id="5b184-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="5b184-139">deviceId</span></span>|<span data-ttu-id="5b184-140">Guid</span><span class="sxs-lookup"><span data-stu-id="5b184-140">Guid</span></span>|<span data-ttu-id="5b184-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5b184-141">Not yet documented</span></span>|
|<span data-ttu-id="5b184-142">профилеид</span><span class="sxs-lookup"><span data-stu-id="5b184-142">profileId</span></span>|<span data-ttu-id="5b184-143">GUID</span><span class="sxs-lookup"><span data-stu-id="5b184-143">Guid</span></span>|<span data-ttu-id="5b184-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5b184-144">Not yet documented</span></span>|
|<span data-ttu-id="5b184-145">отпечаток</span><span class="sxs-lookup"><span data-stu-id="5b184-145">thumbprint</span></span>|<span data-ttu-id="5b184-146">String</span><span class="sxs-lookup"><span data-stu-id="5b184-146">String</span></span>|<span data-ttu-id="5b184-147">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5b184-147">Not yet documented</span></span>|
|<span data-ttu-id="5b184-148">девицекэйсумбпринт</span><span class="sxs-lookup"><span data-stu-id="5b184-148">deviceKeyThumbprint</span></span>|<span data-ttu-id="5b184-149">String</span><span class="sxs-lookup"><span data-stu-id="5b184-149">String</span></span>|<span data-ttu-id="5b184-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5b184-150">Not yet documented</span></span>|
|<span data-ttu-id="5b184-151">status</span><span class="sxs-lookup"><span data-stu-id="5b184-151">status</span></span>|<span data-ttu-id="5b184-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5b184-152">Int32</span></span>|<span data-ttu-id="5b184-153">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="5b184-153">Not yet documented</span></span>|
|<span data-ttu-id="5b184-154">sourceType</span><span class="sxs-lookup"><span data-stu-id="5b184-154">sourceType</span></span>|<span data-ttu-id="5b184-155">Int32</span><span class="sxs-lookup"><span data-stu-id="5b184-155">Int32</span></span>|<span data-ttu-id="5b184-156">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="5b184-156">Not yet documented</span></span>|
|<span data-ttu-id="5b184-157">createdTime</span><span class="sxs-lookup"><span data-stu-id="5b184-157">createdTime</span></span>|<span data-ttu-id="5b184-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b184-158">DateTimeOffset</span></span>|<span data-ttu-id="5b184-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5b184-159">Not yet documented</span></span>|
|<span data-ttu-id="5b184-160">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="5b184-160">lastModifiedTime</span></span>|<span data-ttu-id="5b184-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b184-161">DateTimeOffset</span></span>|<span data-ttu-id="5b184-162">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5b184-162">Not yet documented</span></span>|
|<span data-ttu-id="5b184-163">isDeleted</span><span class="sxs-lookup"><span data-stu-id="5b184-163">isDeleted</span></span>|<span data-ttu-id="5b184-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b184-164">Boolean</span></span>|<span data-ttu-id="5b184-165">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="5b184-165">Not yet documented</span></span>|
|<span data-ttu-id="5b184-166">eTag</span><span class="sxs-lookup"><span data-stu-id="5b184-166">eTag</span></span>|<span data-ttu-id="5b184-167">String</span><span class="sxs-lookup"><span data-stu-id="5b184-167">String</span></span>|<span data-ttu-id="5b184-168">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5b184-168">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5b184-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b184-169">Response</span></span>
<span data-ttu-id="5b184-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b184-170">If successful, this method returns a `200 OK` response code and an updated [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b184-171">Пример</span><span class="sxs-lookup"><span data-stu-id="5b184-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b184-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b184-172">Request</span></span>
<span data-ttu-id="5b184-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b184-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b184-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b184-174">Response</span></span>
<span data-ttu-id="5b184-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b184-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



