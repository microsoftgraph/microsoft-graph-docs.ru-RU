---
title: Создание pfxRecryptionRequest
description: Создайте новый объект pfxRecryptionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eec6a97c73f707743d607414c47b939e0e5cb388
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868866"
---
# <a name="create-pfxrecryptionrequest"></a><span data-ttu-id="3a137-103">Создание pfxRecryptionRequest</span><span class="sxs-lookup"><span data-stu-id="3a137-103">Create pfxRecryptionRequest</span></span>

<span data-ttu-id="3a137-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a137-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a137-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a137-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a137-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a137-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a137-107">Создайте новый [объект pfxRecryptionRequest.](../resources/intune-raimportcerts-pfxrecryptionrequest.md)</span><span class="sxs-lookup"><span data-stu-id="3a137-107">Create a new [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a137-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3a137-108">Prerequisites</span></span>
<span data-ttu-id="3a137-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a137-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a137-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a137-111">Permission type</span></span>|<span data-ttu-id="3a137-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a137-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a137-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a137-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a137-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a137-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3a137-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a137-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a137-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a137-116">Not supported.</span></span>|
|<span data-ttu-id="3a137-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="3a137-117">Application</span></span>|<span data-ttu-id="3a137-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a137-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a137-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a137-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxRecryptionRequests
```

## <a name="request-headers"></a><span data-ttu-id="3a137-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3a137-120">Request headers</span></span>
|<span data-ttu-id="3a137-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a137-121">Header</span></span>|<span data-ttu-id="3a137-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3a137-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a137-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a137-123">Authorization</span></span>|<span data-ttu-id="3a137-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a137-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a137-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a137-125">Accept</span></span>|<span data-ttu-id="3a137-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a137-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a137-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a137-127">Request body</span></span>
<span data-ttu-id="3a137-128">В теле запроса поставляем представление JSON для объекта pfxRecryptionRequest.</span><span class="sxs-lookup"><span data-stu-id="3a137-128">In the request body, supply a JSON representation for the pfxRecryptionRequest object.</span></span>

<span data-ttu-id="3a137-129">В следующей таблице показаны свойства, необходимые при создании pfxRecryptionRequest.</span><span class="sxs-lookup"><span data-stu-id="3a137-129">The following table shows the properties that are required when you create the pfxRecryptionRequest.</span></span>

|<span data-ttu-id="3a137-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a137-130">Property</span></span>|<span data-ttu-id="3a137-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3a137-131">Type</span></span>|<span data-ttu-id="3a137-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3a137-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a137-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="3a137-133">tenantId</span></span>|<span data-ttu-id="3a137-134">Guid</span><span class="sxs-lookup"><span data-stu-id="3a137-134">Guid</span></span>|<span data-ttu-id="3a137-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3a137-135">Not yet documented</span></span>|
|<span data-ttu-id="3a137-136">userId</span><span class="sxs-lookup"><span data-stu-id="3a137-136">userId</span></span>|<span data-ttu-id="3a137-137">Guid</span><span class="sxs-lookup"><span data-stu-id="3a137-137">Guid</span></span>|<span data-ttu-id="3a137-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3a137-138">Not yet documented</span></span>|
|<span data-ttu-id="3a137-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="3a137-139">deviceId</span></span>|<span data-ttu-id="3a137-140">Guid</span><span class="sxs-lookup"><span data-stu-id="3a137-140">Guid</span></span>|<span data-ttu-id="3a137-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3a137-141">Not yet documented</span></span>|
|<span data-ttu-id="3a137-142">profileId</span><span class="sxs-lookup"><span data-stu-id="3a137-142">profileId</span></span>|<span data-ttu-id="3a137-143">Guid</span><span class="sxs-lookup"><span data-stu-id="3a137-143">Guid</span></span>|<span data-ttu-id="3a137-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3a137-144">Not yet documented</span></span>|
|<span data-ttu-id="3a137-145">отпечатки пальцев</span><span class="sxs-lookup"><span data-stu-id="3a137-145">thumbprint</span></span>|<span data-ttu-id="3a137-146">String</span><span class="sxs-lookup"><span data-stu-id="3a137-146">String</span></span>|<span data-ttu-id="3a137-147">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3a137-147">Not yet documented</span></span>|
|<span data-ttu-id="3a137-148">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="3a137-148">deviceKeyThumbprint</span></span>|<span data-ttu-id="3a137-149">String</span><span class="sxs-lookup"><span data-stu-id="3a137-149">String</span></span>|<span data-ttu-id="3a137-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3a137-150">Not yet documented</span></span>|
|<span data-ttu-id="3a137-151">status</span><span class="sxs-lookup"><span data-stu-id="3a137-151">status</span></span>|<span data-ttu-id="3a137-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3a137-152">Int32</span></span>|<span data-ttu-id="3a137-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3a137-153">Not yet documented</span></span>|
|<span data-ttu-id="3a137-154">sourceType</span><span class="sxs-lookup"><span data-stu-id="3a137-154">sourceType</span></span>|<span data-ttu-id="3a137-155">Int32</span><span class="sxs-lookup"><span data-stu-id="3a137-155">Int32</span></span>|<span data-ttu-id="3a137-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3a137-156">Not yet documented</span></span>|
|<span data-ttu-id="3a137-157">createdTime</span><span class="sxs-lookup"><span data-stu-id="3a137-157">createdTime</span></span>|<span data-ttu-id="3a137-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a137-158">DateTimeOffset</span></span>|<span data-ttu-id="3a137-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3a137-159">Not yet documented</span></span>|
|<span data-ttu-id="3a137-160">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="3a137-160">lastModifiedTime</span></span>|<span data-ttu-id="3a137-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a137-161">DateTimeOffset</span></span>|<span data-ttu-id="3a137-162">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3a137-162">Not yet documented</span></span>|
|<span data-ttu-id="3a137-163">isDeleted</span><span class="sxs-lookup"><span data-stu-id="3a137-163">isDeleted</span></span>|<span data-ttu-id="3a137-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a137-164">Boolean</span></span>|<span data-ttu-id="3a137-165">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3a137-165">Not yet documented</span></span>|
|<span data-ttu-id="3a137-166">eTag</span><span class="sxs-lookup"><span data-stu-id="3a137-166">eTag</span></span>|<span data-ttu-id="3a137-167">String</span><span class="sxs-lookup"><span data-stu-id="3a137-167">String</span></span>|<span data-ttu-id="3a137-168">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3a137-168">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3a137-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a137-169">Response</span></span>
<span data-ttu-id="3a137-170">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3a137-170">If successful, this method returns a `201 Created` response code and a [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a137-171">Пример</span><span class="sxs-lookup"><span data-stu-id="3a137-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a137-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a137-172">Request</span></span>
<span data-ttu-id="3a137-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a137-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3a137-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a137-174">Response</span></span>
<span data-ttu-id="3a137-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a137-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




