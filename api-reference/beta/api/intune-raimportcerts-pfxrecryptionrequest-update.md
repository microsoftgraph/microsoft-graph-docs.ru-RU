---
title: Обновление Пфксрекриптионрекуест
description: Обновление свойств объекта Пфксрекриптионрекуест.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca4addaae01a6fea69d1742338e0452ed7227380
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741484"
---
# <a name="update-pfxrecryptionrequest"></a><span data-ttu-id="99c97-103">Обновление Пфксрекриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="99c97-103">Update pfxRecryptionRequest</span></span>

> <span data-ttu-id="99c97-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99c97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99c97-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99c97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99c97-106">Обновление свойств объекта [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="99c97-106">Update the properties of a [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99c97-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="99c97-107">Prerequisites</span></span>
<span data-ttu-id="99c97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99c97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99c97-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99c97-110">Permission type</span></span>|<span data-ttu-id="99c97-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="99c97-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99c97-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99c97-112">Delegated (work or school account)</span></span>|<span data-ttu-id="99c97-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99c97-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="99c97-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99c97-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99c97-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99c97-115">Not supported.</span></span>|
|<span data-ttu-id="99c97-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99c97-116">Application</span></span>|<span data-ttu-id="99c97-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99c97-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99c97-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99c97-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxRecryptionRequests/{pfxRecryptionRequestsId}
```

## <a name="request-headers"></a><span data-ttu-id="99c97-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99c97-119">Request headers</span></span>
|<span data-ttu-id="99c97-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="99c97-120">Header</span></span>|<span data-ttu-id="99c97-121">Значение</span><span class="sxs-lookup"><span data-stu-id="99c97-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99c97-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99c97-122">Authorization</span></span>|<span data-ttu-id="99c97-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99c97-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99c97-124">Accept</span><span class="sxs-lookup"><span data-stu-id="99c97-124">Accept</span></span>|<span data-ttu-id="99c97-125">application/json</span><span class="sxs-lookup"><span data-stu-id="99c97-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99c97-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="99c97-126">Request body</span></span>
<span data-ttu-id="99c97-127">В тексте запроса добавьте представление объекта [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99c97-127">In the request body, supply a JSON representation for the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

<span data-ttu-id="99c97-128">В следующей таблице приведены свойства, необходимые при создании [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md).</span><span class="sxs-lookup"><span data-stu-id="99c97-128">The following table shows the properties that are required when you create the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md).</span></span>

|<span data-ttu-id="99c97-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="99c97-129">Property</span></span>|<span data-ttu-id="99c97-130">Тип</span><span class="sxs-lookup"><span data-stu-id="99c97-130">Type</span></span>|<span data-ttu-id="99c97-131">Описание</span><span class="sxs-lookup"><span data-stu-id="99c97-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99c97-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="99c97-132">tenantId</span></span>|<span data-ttu-id="99c97-133">GUID</span><span class="sxs-lookup"><span data-stu-id="99c97-133">Guid</span></span>|<span data-ttu-id="99c97-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="99c97-134">Not yet documented</span></span>|
|<span data-ttu-id="99c97-135">userId</span><span class="sxs-lookup"><span data-stu-id="99c97-135">userId</span></span>|<span data-ttu-id="99c97-136">GUID</span><span class="sxs-lookup"><span data-stu-id="99c97-136">Guid</span></span>|<span data-ttu-id="99c97-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="99c97-137">Not yet documented</span></span>|
|<span data-ttu-id="99c97-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="99c97-138">deviceId</span></span>|<span data-ttu-id="99c97-139">Guid</span><span class="sxs-lookup"><span data-stu-id="99c97-139">Guid</span></span>|<span data-ttu-id="99c97-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="99c97-140">Not yet documented</span></span>|
|<span data-ttu-id="99c97-141">Профилеид</span><span class="sxs-lookup"><span data-stu-id="99c97-141">profileId</span></span>|<span data-ttu-id="99c97-142">GUID</span><span class="sxs-lookup"><span data-stu-id="99c97-142">Guid</span></span>|<span data-ttu-id="99c97-143">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="99c97-143">Not yet documented</span></span>|
|<span data-ttu-id="99c97-144">отпечаток</span><span class="sxs-lookup"><span data-stu-id="99c97-144">thumbprint</span></span>|<span data-ttu-id="99c97-145">String</span><span class="sxs-lookup"><span data-stu-id="99c97-145">String</span></span>|<span data-ttu-id="99c97-146">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="99c97-146">Not yet documented</span></span>|
|<span data-ttu-id="99c97-147">Девицекэйсумбпринт</span><span class="sxs-lookup"><span data-stu-id="99c97-147">deviceKeyThumbprint</span></span>|<span data-ttu-id="99c97-148">String</span><span class="sxs-lookup"><span data-stu-id="99c97-148">String</span></span>|<span data-ttu-id="99c97-149">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="99c97-149">Not yet documented</span></span>|
|<span data-ttu-id="99c97-150">status</span><span class="sxs-lookup"><span data-stu-id="99c97-150">status</span></span>|<span data-ttu-id="99c97-151">Int32</span><span class="sxs-lookup"><span data-stu-id="99c97-151">Int32</span></span>|<span data-ttu-id="99c97-152">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="99c97-152">Not yet documented</span></span>|
|<span data-ttu-id="99c97-153">sourceType</span><span class="sxs-lookup"><span data-stu-id="99c97-153">sourceType</span></span>|<span data-ttu-id="99c97-154">Int32</span><span class="sxs-lookup"><span data-stu-id="99c97-154">Int32</span></span>|<span data-ttu-id="99c97-155">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="99c97-155">Not yet documented</span></span>|
|<span data-ttu-id="99c97-156">createdTime</span><span class="sxs-lookup"><span data-stu-id="99c97-156">createdTime</span></span>|<span data-ttu-id="99c97-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99c97-157">DateTimeOffset</span></span>|<span data-ttu-id="99c97-158">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="99c97-158">Not yet documented</span></span>|
|<span data-ttu-id="99c97-159">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="99c97-159">lastModifiedTime</span></span>|<span data-ttu-id="99c97-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99c97-160">DateTimeOffset</span></span>|<span data-ttu-id="99c97-161">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="99c97-161">Not yet documented</span></span>|
|<span data-ttu-id="99c97-162">isDeleted</span><span class="sxs-lookup"><span data-stu-id="99c97-162">isDeleted</span></span>|<span data-ttu-id="99c97-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="99c97-163">Boolean</span></span>|<span data-ttu-id="99c97-164">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="99c97-164">Not yet documented</span></span>|
|<span data-ttu-id="99c97-165">eTag</span><span class="sxs-lookup"><span data-stu-id="99c97-165">eTag</span></span>|<span data-ttu-id="99c97-166">String</span><span class="sxs-lookup"><span data-stu-id="99c97-166">String</span></span>|<span data-ttu-id="99c97-167">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="99c97-167">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="99c97-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="99c97-168">Response</span></span>
<span data-ttu-id="99c97-169">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="99c97-169">If successful, this method returns a `200 OK` response code and an updated [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99c97-170">Пример</span><span class="sxs-lookup"><span data-stu-id="99c97-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="99c97-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="99c97-171">Request</span></span>
<span data-ttu-id="99c97-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99c97-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="99c97-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="99c97-173">Response</span></span>
<span data-ttu-id="99c97-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="99c97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





