---
title: Обновление pfxUserCertificate
description: Обновление свойств объекта pfxUserCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1543bb29e379458b15a7ebb915e0e32d4c6bacc2
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868833"
---
# <a name="update-pfxusercertificate"></a><span data-ttu-id="2d881-103">Обновление pfxUserCertificate</span><span class="sxs-lookup"><span data-stu-id="2d881-103">Update pfxUserCertificate</span></span>

<span data-ttu-id="2d881-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d881-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d881-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d881-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d881-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d881-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d881-107">Обновление свойств объекта [pfxUserCertificate.](../resources/intune-raimportcerts-pfxusercertificate.md)</span><span class="sxs-lookup"><span data-stu-id="2d881-107">Update the properties of a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d881-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2d881-108">Prerequisites</span></span>
<span data-ttu-id="2d881-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d881-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d881-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d881-111">Permission type</span></span>|<span data-ttu-id="2d881-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d881-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d881-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d881-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2d881-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d881-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d881-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d881-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d881-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d881-116">Not supported.</span></span>|
|<span data-ttu-id="2d881-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="2d881-117">Application</span></span>|<span data-ttu-id="2d881-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d881-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d881-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d881-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxUserCertificates/{pfxUserCertificatesId}
```

## <a name="request-headers"></a><span data-ttu-id="2d881-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2d881-120">Request headers</span></span>
|<span data-ttu-id="2d881-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2d881-121">Header</span></span>|<span data-ttu-id="2d881-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2d881-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d881-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d881-123">Authorization</span></span>|<span data-ttu-id="2d881-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d881-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d881-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2d881-125">Accept</span></span>|<span data-ttu-id="2d881-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2d881-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d881-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d881-127">Request body</span></span>
<span data-ttu-id="2d881-128">В теле запроса поставляем представление JSON для [объекта pfxUserCertificate.](../resources/intune-raimportcerts-pfxusercertificate.md)</span><span class="sxs-lookup"><span data-stu-id="2d881-128">In the request body, supply a JSON representation for the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

<span data-ttu-id="2d881-129">В следующей таблице показаны свойства, необходимые при создании [pfxUserCertificate.](../resources/intune-raimportcerts-pfxusercertificate.md)</span><span class="sxs-lookup"><span data-stu-id="2d881-129">The following table shows the properties that are required when you create the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md).</span></span>

|<span data-ttu-id="2d881-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d881-130">Property</span></span>|<span data-ttu-id="2d881-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2d881-131">Type</span></span>|<span data-ttu-id="2d881-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2d881-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d881-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="2d881-133">tenantId</span></span>|<span data-ttu-id="2d881-134">Guid</span><span class="sxs-lookup"><span data-stu-id="2d881-134">Guid</span></span>|<span data-ttu-id="2d881-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d881-135">Not yet documented</span></span>|
|<span data-ttu-id="2d881-136">userId</span><span class="sxs-lookup"><span data-stu-id="2d881-136">userId</span></span>|<span data-ttu-id="2d881-137">Guid</span><span class="sxs-lookup"><span data-stu-id="2d881-137">Guid</span></span>|<span data-ttu-id="2d881-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d881-138">Not yet documented</span></span>|
|<span data-ttu-id="2d881-139">отпечатки пальцев</span><span class="sxs-lookup"><span data-stu-id="2d881-139">thumbprint</span></span>|<span data-ttu-id="2d881-140">String</span><span class="sxs-lookup"><span data-stu-id="2d881-140">String</span></span>|<span data-ttu-id="2d881-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d881-141">Not yet documented</span></span>|
|<span data-ttu-id="2d881-142">userUpn</span><span class="sxs-lookup"><span data-stu-id="2d881-142">userUpn</span></span>|<span data-ttu-id="2d881-143">String</span><span class="sxs-lookup"><span data-stu-id="2d881-143">String</span></span>|<span data-ttu-id="2d881-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d881-144">Not yet documented</span></span>|
|<span data-ttu-id="2d881-145">зашифрованныйPfxBlob</span><span class="sxs-lookup"><span data-stu-id="2d881-145">encryptedPfxBlob</span></span>|<span data-ttu-id="2d881-146">String</span><span class="sxs-lookup"><span data-stu-id="2d881-146">String</span></span>|<span data-ttu-id="2d881-147">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d881-147">Not yet documented</span></span>|
|<span data-ttu-id="2d881-148">зашифрованныйPfxPassword</span><span class="sxs-lookup"><span data-stu-id="2d881-148">encryptedPfxPassword</span></span>|<span data-ttu-id="2d881-149">String</span><span class="sxs-lookup"><span data-stu-id="2d881-149">String</span></span>|<span data-ttu-id="2d881-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d881-150">Not yet documented</span></span>|
|<span data-ttu-id="2d881-151">certStartDate</span><span class="sxs-lookup"><span data-stu-id="2d881-151">certStartDate</span></span>|<span data-ttu-id="2d881-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d881-152">DateTimeOffset</span></span>|<span data-ttu-id="2d881-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d881-153">Not yet documented</span></span>|
|<span data-ttu-id="2d881-154">certExpirationDate</span><span class="sxs-lookup"><span data-stu-id="2d881-154">certExpirationDate</span></span>|<span data-ttu-id="2d881-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d881-155">DateTimeOffset</span></span>|<span data-ttu-id="2d881-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d881-156">Not yet documented</span></span>|
|<span data-ttu-id="2d881-157">providerName</span><span class="sxs-lookup"><span data-stu-id="2d881-157">providerName</span></span>|<span data-ttu-id="2d881-158">String</span><span class="sxs-lookup"><span data-stu-id="2d881-158">String</span></span>|<span data-ttu-id="2d881-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d881-159">Not yet documented</span></span>|
|<span data-ttu-id="2d881-160">encryptionKeyName</span><span class="sxs-lookup"><span data-stu-id="2d881-160">encryptionKeyName</span></span>|<span data-ttu-id="2d881-161">String</span><span class="sxs-lookup"><span data-stu-id="2d881-161">String</span></span>|<span data-ttu-id="2d881-162">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d881-162">Not yet documented</span></span>|
|<span data-ttu-id="2d881-163">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="2d881-163">paddingScheme</span></span>|<span data-ttu-id="2d881-164">Int32</span><span class="sxs-lookup"><span data-stu-id="2d881-164">Int32</span></span>|<span data-ttu-id="2d881-165">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d881-165">Not yet documented</span></span>|
|<span data-ttu-id="2d881-166">status</span><span class="sxs-lookup"><span data-stu-id="2d881-166">status</span></span>|<span data-ttu-id="2d881-167">Int32</span><span class="sxs-lookup"><span data-stu-id="2d881-167">Int32</span></span>|<span data-ttu-id="2d881-168">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d881-168">Not yet documented</span></span>|
|<span data-ttu-id="2d881-169">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="2d881-169">intendedPurpose</span></span>|<span data-ttu-id="2d881-170">Int32</span><span class="sxs-lookup"><span data-stu-id="2d881-170">Int32</span></span>|<span data-ttu-id="2d881-171">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d881-171">Not yet documented</span></span>|
|<span data-ttu-id="2d881-172">createdTime</span><span class="sxs-lookup"><span data-stu-id="2d881-172">createdTime</span></span>|<span data-ttu-id="2d881-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d881-173">DateTimeOffset</span></span>|<span data-ttu-id="2d881-174">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d881-174">Not yet documented</span></span>|
|<span data-ttu-id="2d881-175">isDeleted</span><span class="sxs-lookup"><span data-stu-id="2d881-175">isDeleted</span></span>|<span data-ttu-id="2d881-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d881-176">Boolean</span></span>|<span data-ttu-id="2d881-177">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2d881-177">Not yet documented</span></span>|
|<span data-ttu-id="2d881-178">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="2d881-178">lastModifiedTime</span></span>|<span data-ttu-id="2d881-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d881-179">DateTimeOffset</span></span>|<span data-ttu-id="2d881-180">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d881-180">Not yet documented</span></span>|
|<span data-ttu-id="2d881-181">eTag</span><span class="sxs-lookup"><span data-stu-id="2d881-181">eTag</span></span>|<span data-ttu-id="2d881-182">String</span><span class="sxs-lookup"><span data-stu-id="2d881-182">String</span></span>|<span data-ttu-id="2d881-183">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d881-183">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2d881-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="2d881-184">Response</span></span>
<span data-ttu-id="2d881-185">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2d881-185">If successful, this method returns a `200 OK` response code and an updated [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d881-186">Пример</span><span class="sxs-lookup"><span data-stu-id="2d881-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d881-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d881-187">Request</span></span>
<span data-ttu-id="2d881-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d881-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/pfxUserCertificates/{pfxUserCertificatesId}
Content-type: application/json
Content-length: 789

{
  "@odata.type": "#microsoft.graph.pfxUserCertificate",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "thumbprint": "Thumbprint value",
  "userUpn": "User Upn value",
  "encryptedPfxBlob": "Encrypted Pfx Blob value",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "certStartDate": "2017-01-01T00:01:48.7697664-08:00",
  "certExpirationDate": "2016-12-31T23:56:39.3841403-08:00",
  "providerName": "Provider Name value",
  "encryptionKeyName": "Encryption Key Name value",
  "paddingScheme": 13,
  "status": 6,
  "intendedPurpose": 15,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "isDeleted": true,
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value"
}
```

### <a name="response"></a><span data-ttu-id="2d881-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d881-189">Response</span></span>
<span data-ttu-id="2d881-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d881-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 789

{
  "@odata.type": "#microsoft.graph.pfxUserCertificate",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "thumbprint": "Thumbprint value",
  "userUpn": "User Upn value",
  "encryptedPfxBlob": "Encrypted Pfx Blob value",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "certStartDate": "2017-01-01T00:01:48.7697664-08:00",
  "certExpirationDate": "2016-12-31T23:56:39.3841403-08:00",
  "providerName": "Provider Name value",
  "encryptionKeyName": "Encryption Key Name value",
  "paddingScheme": 13,
  "status": 6,
  "intendedPurpose": 15,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "isDeleted": true,
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value"
}
```




