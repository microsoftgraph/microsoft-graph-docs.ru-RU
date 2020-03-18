---
title: Создание Пфксусерцертификате
description: Создание нового объекта Пфксусерцертификате.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5b320c1d7893fabc824ec3c5c6a456df3bc45b26
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801882"
---
# <a name="create-pfxusercertificate"></a><span data-ttu-id="011ee-103">Создание Пфксусерцертификате</span><span class="sxs-lookup"><span data-stu-id="011ee-103">Create pfxUserCertificate</span></span>

> <span data-ttu-id="011ee-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="011ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="011ee-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="011ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="011ee-106">Создание нового объекта [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="011ee-106">Create a new [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="011ee-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="011ee-107">Prerequisites</span></span>
<span data-ttu-id="011ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="011ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="011ee-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="011ee-110">Permission type</span></span>|<span data-ttu-id="011ee-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="011ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="011ee-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="011ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="011ee-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="011ee-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="011ee-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="011ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="011ee-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="011ee-115">Not supported.</span></span>|
|<span data-ttu-id="011ee-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="011ee-116">Application</span></span>|<span data-ttu-id="011ee-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="011ee-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="011ee-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="011ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxUserCertificates
```

## <a name="request-headers"></a><span data-ttu-id="011ee-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="011ee-119">Request headers</span></span>
|<span data-ttu-id="011ee-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="011ee-120">Header</span></span>|<span data-ttu-id="011ee-121">Значение</span><span class="sxs-lookup"><span data-stu-id="011ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="011ee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="011ee-122">Authorization</span></span>|<span data-ttu-id="011ee-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="011ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="011ee-124">Accept</span><span class="sxs-lookup"><span data-stu-id="011ee-124">Accept</span></span>|<span data-ttu-id="011ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="011ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="011ee-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="011ee-126">Request body</span></span>
<span data-ttu-id="011ee-127">В тексте запроса добавьте представление объекта Пфксусерцертификате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="011ee-127">In the request body, supply a JSON representation for the pfxUserCertificate object.</span></span>

<span data-ttu-id="011ee-128">В следующей таблице приведены свойства, необходимые при создании Пфксусерцертификате.</span><span class="sxs-lookup"><span data-stu-id="011ee-128">The following table shows the properties that are required when you create the pfxUserCertificate.</span></span>

|<span data-ttu-id="011ee-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="011ee-129">Property</span></span>|<span data-ttu-id="011ee-130">Тип</span><span class="sxs-lookup"><span data-stu-id="011ee-130">Type</span></span>|<span data-ttu-id="011ee-131">Описание</span><span class="sxs-lookup"><span data-stu-id="011ee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="011ee-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="011ee-132">tenantId</span></span>|<span data-ttu-id="011ee-133">GUID</span><span class="sxs-lookup"><span data-stu-id="011ee-133">Guid</span></span>|<span data-ttu-id="011ee-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="011ee-134">Not yet documented</span></span>|
|<span data-ttu-id="011ee-135">userId</span><span class="sxs-lookup"><span data-stu-id="011ee-135">userId</span></span>|<span data-ttu-id="011ee-136">GUID</span><span class="sxs-lookup"><span data-stu-id="011ee-136">Guid</span></span>|<span data-ttu-id="011ee-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="011ee-137">Not yet documented</span></span>|
|<span data-ttu-id="011ee-138">отпечаток</span><span class="sxs-lookup"><span data-stu-id="011ee-138">thumbprint</span></span>|<span data-ttu-id="011ee-139">String</span><span class="sxs-lookup"><span data-stu-id="011ee-139">String</span></span>|<span data-ttu-id="011ee-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="011ee-140">Not yet documented</span></span>|
|<span data-ttu-id="011ee-141">усерупн</span><span class="sxs-lookup"><span data-stu-id="011ee-141">userUpn</span></span>|<span data-ttu-id="011ee-142">String</span><span class="sxs-lookup"><span data-stu-id="011ee-142">String</span></span>|<span data-ttu-id="011ee-143">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="011ee-143">Not yet documented</span></span>|
|<span data-ttu-id="011ee-144">енкриптедпфксблоб</span><span class="sxs-lookup"><span data-stu-id="011ee-144">encryptedPfxBlob</span></span>|<span data-ttu-id="011ee-145">String</span><span class="sxs-lookup"><span data-stu-id="011ee-145">String</span></span>|<span data-ttu-id="011ee-146">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="011ee-146">Not yet documented</span></span>|
|<span data-ttu-id="011ee-147">енкриптедпфкспассворд</span><span class="sxs-lookup"><span data-stu-id="011ee-147">encryptedPfxPassword</span></span>|<span data-ttu-id="011ee-148">String</span><span class="sxs-lookup"><span data-stu-id="011ee-148">String</span></span>|<span data-ttu-id="011ee-149">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="011ee-149">Not yet documented</span></span>|
|<span data-ttu-id="011ee-150">цертстартдате</span><span class="sxs-lookup"><span data-stu-id="011ee-150">certStartDate</span></span>|<span data-ttu-id="011ee-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="011ee-151">DateTimeOffset</span></span>|<span data-ttu-id="011ee-152">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="011ee-152">Not yet documented</span></span>|
|<span data-ttu-id="011ee-153">цертекспиратиондате</span><span class="sxs-lookup"><span data-stu-id="011ee-153">certExpirationDate</span></span>|<span data-ttu-id="011ee-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="011ee-154">DateTimeOffset</span></span>|<span data-ttu-id="011ee-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="011ee-155">Not yet documented</span></span>|
|<span data-ttu-id="011ee-156">providerName</span><span class="sxs-lookup"><span data-stu-id="011ee-156">providerName</span></span>|<span data-ttu-id="011ee-157">String</span><span class="sxs-lookup"><span data-stu-id="011ee-157">String</span></span>|<span data-ttu-id="011ee-158">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="011ee-158">Not yet documented</span></span>|
|<span data-ttu-id="011ee-159">енкриптионкэйнаме</span><span class="sxs-lookup"><span data-stu-id="011ee-159">encryptionKeyName</span></span>|<span data-ttu-id="011ee-160">String</span><span class="sxs-lookup"><span data-stu-id="011ee-160">String</span></span>|<span data-ttu-id="011ee-161">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="011ee-161">Not yet documented</span></span>|
|<span data-ttu-id="011ee-162">паддингсчеме</span><span class="sxs-lookup"><span data-stu-id="011ee-162">paddingScheme</span></span>|<span data-ttu-id="011ee-163">Int32</span><span class="sxs-lookup"><span data-stu-id="011ee-163">Int32</span></span>|<span data-ttu-id="011ee-164">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="011ee-164">Not yet documented</span></span>|
|<span data-ttu-id="011ee-165">status</span><span class="sxs-lookup"><span data-stu-id="011ee-165">status</span></span>|<span data-ttu-id="011ee-166">Int32</span><span class="sxs-lookup"><span data-stu-id="011ee-166">Int32</span></span>|<span data-ttu-id="011ee-167">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="011ee-167">Not yet documented</span></span>|
|<span data-ttu-id="011ee-168">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="011ee-168">intendedPurpose</span></span>|<span data-ttu-id="011ee-169">Int32</span><span class="sxs-lookup"><span data-stu-id="011ee-169">Int32</span></span>|<span data-ttu-id="011ee-170">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="011ee-170">Not yet documented</span></span>|
|<span data-ttu-id="011ee-171">createdTime</span><span class="sxs-lookup"><span data-stu-id="011ee-171">createdTime</span></span>|<span data-ttu-id="011ee-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="011ee-172">DateTimeOffset</span></span>|<span data-ttu-id="011ee-173">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="011ee-173">Not yet documented</span></span>|
|<span data-ttu-id="011ee-174">isDeleted</span><span class="sxs-lookup"><span data-stu-id="011ee-174">isDeleted</span></span>|<span data-ttu-id="011ee-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="011ee-175">Boolean</span></span>|<span data-ttu-id="011ee-176">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="011ee-176">Not yet documented</span></span>|
|<span data-ttu-id="011ee-177">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="011ee-177">lastModifiedTime</span></span>|<span data-ttu-id="011ee-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="011ee-178">DateTimeOffset</span></span>|<span data-ttu-id="011ee-179">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="011ee-179">Not yet documented</span></span>|
|<span data-ttu-id="011ee-180">eTag</span><span class="sxs-lookup"><span data-stu-id="011ee-180">eTag</span></span>|<span data-ttu-id="011ee-181">String</span><span class="sxs-lookup"><span data-stu-id="011ee-181">String</span></span>|<span data-ttu-id="011ee-182">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="011ee-182">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="011ee-183">Ответ</span><span class="sxs-lookup"><span data-stu-id="011ee-183">Response</span></span>
<span data-ttu-id="011ee-184">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="011ee-184">If successful, this method returns a `201 Created` response code and a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="011ee-185">Пример</span><span class="sxs-lookup"><span data-stu-id="011ee-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="011ee-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="011ee-186">Request</span></span>
<span data-ttu-id="011ee-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="011ee-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/pfxUserCertificates
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

### <a name="response"></a><span data-ttu-id="011ee-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="011ee-188">Response</span></span>
<span data-ttu-id="011ee-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="011ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




