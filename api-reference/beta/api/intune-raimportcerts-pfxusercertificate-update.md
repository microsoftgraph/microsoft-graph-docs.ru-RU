---
title: Обновление Пфксусерцертификате
description: Обновление свойств объекта Пфксусерцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a4498260afe255b5b71e5d2bcfab44df331e5c24
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460068"
---
# <a name="update-pfxusercertificate"></a><span data-ttu-id="06836-103">Обновление Пфксусерцертификате</span><span class="sxs-lookup"><span data-stu-id="06836-103">Update pfxUserCertificate</span></span>

<span data-ttu-id="06836-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="06836-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06836-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06836-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06836-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06836-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06836-107">Обновление свойств объекта [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="06836-107">Update the properties of a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06836-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="06836-108">Prerequisites</span></span>
<span data-ttu-id="06836-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06836-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06836-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06836-111">Permission type</span></span>|<span data-ttu-id="06836-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="06836-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06836-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06836-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06836-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06836-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06836-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06836-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06836-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06836-116">Not supported.</span></span>|
|<span data-ttu-id="06836-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06836-117">Application</span></span>|<span data-ttu-id="06836-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06836-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06836-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06836-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxUserCertificates/{pfxUserCertificatesId}
```

## <a name="request-headers"></a><span data-ttu-id="06836-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="06836-120">Request headers</span></span>
|<span data-ttu-id="06836-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06836-121">Header</span></span>|<span data-ttu-id="06836-122">Значение</span><span class="sxs-lookup"><span data-stu-id="06836-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06836-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="06836-123">Authorization</span></span>|<span data-ttu-id="06836-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06836-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06836-125">Accept</span><span class="sxs-lookup"><span data-stu-id="06836-125">Accept</span></span>|<span data-ttu-id="06836-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06836-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06836-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06836-127">Request body</span></span>
<span data-ttu-id="06836-128">В тексте запроса добавьте представление объекта [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06836-128">In the request body, supply a JSON representation for the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

<span data-ttu-id="06836-129">В следующей таблице приведены свойства, необходимые при создании [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md).</span><span class="sxs-lookup"><span data-stu-id="06836-129">The following table shows the properties that are required when you create the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md).</span></span>

|<span data-ttu-id="06836-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="06836-130">Property</span></span>|<span data-ttu-id="06836-131">Тип</span><span class="sxs-lookup"><span data-stu-id="06836-131">Type</span></span>|<span data-ttu-id="06836-132">Описание</span><span class="sxs-lookup"><span data-stu-id="06836-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06836-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="06836-133">tenantId</span></span>|<span data-ttu-id="06836-134">GUID</span><span class="sxs-lookup"><span data-stu-id="06836-134">Guid</span></span>|<span data-ttu-id="06836-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06836-135">Not yet documented</span></span>|
|<span data-ttu-id="06836-136">userId</span><span class="sxs-lookup"><span data-stu-id="06836-136">userId</span></span>|<span data-ttu-id="06836-137">GUID</span><span class="sxs-lookup"><span data-stu-id="06836-137">Guid</span></span>|<span data-ttu-id="06836-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06836-138">Not yet documented</span></span>|
|<span data-ttu-id="06836-139">отпечаток</span><span class="sxs-lookup"><span data-stu-id="06836-139">thumbprint</span></span>|<span data-ttu-id="06836-140">String</span><span class="sxs-lookup"><span data-stu-id="06836-140">String</span></span>|<span data-ttu-id="06836-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06836-141">Not yet documented</span></span>|
|<span data-ttu-id="06836-142">усерупн</span><span class="sxs-lookup"><span data-stu-id="06836-142">userUpn</span></span>|<span data-ttu-id="06836-143">String</span><span class="sxs-lookup"><span data-stu-id="06836-143">String</span></span>|<span data-ttu-id="06836-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06836-144">Not yet documented</span></span>|
|<span data-ttu-id="06836-145">енкриптедпфксблоб</span><span class="sxs-lookup"><span data-stu-id="06836-145">encryptedPfxBlob</span></span>|<span data-ttu-id="06836-146">String</span><span class="sxs-lookup"><span data-stu-id="06836-146">String</span></span>|<span data-ttu-id="06836-147">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06836-147">Not yet documented</span></span>|
|<span data-ttu-id="06836-148">енкриптедпфкспассворд</span><span class="sxs-lookup"><span data-stu-id="06836-148">encryptedPfxPassword</span></span>|<span data-ttu-id="06836-149">String</span><span class="sxs-lookup"><span data-stu-id="06836-149">String</span></span>|<span data-ttu-id="06836-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06836-150">Not yet documented</span></span>|
|<span data-ttu-id="06836-151">цертстартдате</span><span class="sxs-lookup"><span data-stu-id="06836-151">certStartDate</span></span>|<span data-ttu-id="06836-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06836-152">DateTimeOffset</span></span>|<span data-ttu-id="06836-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06836-153">Not yet documented</span></span>|
|<span data-ttu-id="06836-154">цертекспиратиондате</span><span class="sxs-lookup"><span data-stu-id="06836-154">certExpirationDate</span></span>|<span data-ttu-id="06836-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06836-155">DateTimeOffset</span></span>|<span data-ttu-id="06836-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06836-156">Not yet documented</span></span>|
|<span data-ttu-id="06836-157">providerName</span><span class="sxs-lookup"><span data-stu-id="06836-157">providerName</span></span>|<span data-ttu-id="06836-158">String</span><span class="sxs-lookup"><span data-stu-id="06836-158">String</span></span>|<span data-ttu-id="06836-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06836-159">Not yet documented</span></span>|
|<span data-ttu-id="06836-160">енкриптионкэйнаме</span><span class="sxs-lookup"><span data-stu-id="06836-160">encryptionKeyName</span></span>|<span data-ttu-id="06836-161">String</span><span class="sxs-lookup"><span data-stu-id="06836-161">String</span></span>|<span data-ttu-id="06836-162">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06836-162">Not yet documented</span></span>|
|<span data-ttu-id="06836-163">паддингсчеме</span><span class="sxs-lookup"><span data-stu-id="06836-163">paddingScheme</span></span>|<span data-ttu-id="06836-164">Int32</span><span class="sxs-lookup"><span data-stu-id="06836-164">Int32</span></span>|<span data-ttu-id="06836-165">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="06836-165">Not yet documented</span></span>|
|<span data-ttu-id="06836-166">status</span><span class="sxs-lookup"><span data-stu-id="06836-166">status</span></span>|<span data-ttu-id="06836-167">Int32</span><span class="sxs-lookup"><span data-stu-id="06836-167">Int32</span></span>|<span data-ttu-id="06836-168">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="06836-168">Not yet documented</span></span>|
|<span data-ttu-id="06836-169">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="06836-169">intendedPurpose</span></span>|<span data-ttu-id="06836-170">Int32</span><span class="sxs-lookup"><span data-stu-id="06836-170">Int32</span></span>|<span data-ttu-id="06836-171">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="06836-171">Not yet documented</span></span>|
|<span data-ttu-id="06836-172">createdTime</span><span class="sxs-lookup"><span data-stu-id="06836-172">createdTime</span></span>|<span data-ttu-id="06836-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06836-173">DateTimeOffset</span></span>|<span data-ttu-id="06836-174">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06836-174">Not yet documented</span></span>|
|<span data-ttu-id="06836-175">isDeleted</span><span class="sxs-lookup"><span data-stu-id="06836-175">isDeleted</span></span>|<span data-ttu-id="06836-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="06836-176">Boolean</span></span>|<span data-ttu-id="06836-177">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="06836-177">Not yet documented</span></span>|
|<span data-ttu-id="06836-178">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="06836-178">lastModifiedTime</span></span>|<span data-ttu-id="06836-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06836-179">DateTimeOffset</span></span>|<span data-ttu-id="06836-180">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06836-180">Not yet documented</span></span>|
|<span data-ttu-id="06836-181">eTag</span><span class="sxs-lookup"><span data-stu-id="06836-181">eTag</span></span>|<span data-ttu-id="06836-182">String</span><span class="sxs-lookup"><span data-stu-id="06836-182">String</span></span>|<span data-ttu-id="06836-183">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06836-183">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="06836-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="06836-184">Response</span></span>
<span data-ttu-id="06836-185">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06836-185">If successful, this method returns a `200 OK` response code and an updated [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06836-186">Пример</span><span class="sxs-lookup"><span data-stu-id="06836-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="06836-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="06836-187">Request</span></span>
<span data-ttu-id="06836-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06836-188">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="06836-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="06836-189">Response</span></span>
<span data-ttu-id="06836-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06836-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





