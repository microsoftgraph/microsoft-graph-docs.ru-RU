---
title: Создание Пфксусерцертификате
description: Создание нового объекта Пфксусерцертификате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 15ce1610e1b67782a347d8b85013a0faf544c19d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093177"
---
# <a name="create-pfxusercertificate"></a><span data-ttu-id="0fbca-103">Создание Пфксусерцертификате</span><span class="sxs-lookup"><span data-stu-id="0fbca-103">Create pfxUserCertificate</span></span>

<span data-ttu-id="0fbca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fbca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0fbca-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fbca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fbca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0fbca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fbca-107">Создание нового объекта [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="0fbca-107">Create a new [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fbca-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0fbca-108">Prerequisites</span></span>
<span data-ttu-id="0fbca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fbca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fbca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fbca-111">Permission type</span></span>|<span data-ttu-id="0fbca-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fbca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fbca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fbca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0fbca-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fbca-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0fbca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fbca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fbca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fbca-116">Not supported.</span></span>|
|<span data-ttu-id="0fbca-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fbca-117">Application</span></span>|<span data-ttu-id="0fbca-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fbca-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fbca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fbca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxUserCertificates
```

## <a name="request-headers"></a><span data-ttu-id="0fbca-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0fbca-120">Request headers</span></span>
|<span data-ttu-id="0fbca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0fbca-121">Header</span></span>|<span data-ttu-id="0fbca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0fbca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fbca-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0fbca-123">Authorization</span></span>|<span data-ttu-id="0fbca-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fbca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fbca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0fbca-125">Accept</span></span>|<span data-ttu-id="0fbca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0fbca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fbca-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0fbca-127">Request body</span></span>
<span data-ttu-id="0fbca-128">В тексте запроса добавьте представление объекта Пфксусерцертификате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0fbca-128">In the request body, supply a JSON representation for the pfxUserCertificate object.</span></span>

<span data-ttu-id="0fbca-129">В следующей таблице приведены свойства, необходимые при создании Пфксусерцертификате.</span><span class="sxs-lookup"><span data-stu-id="0fbca-129">The following table shows the properties that are required when you create the pfxUserCertificate.</span></span>

|<span data-ttu-id="0fbca-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0fbca-130">Property</span></span>|<span data-ttu-id="0fbca-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0fbca-131">Type</span></span>|<span data-ttu-id="0fbca-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0fbca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fbca-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="0fbca-133">tenantId</span></span>|<span data-ttu-id="0fbca-134">Guid</span><span class="sxs-lookup"><span data-stu-id="0fbca-134">Guid</span></span>|<span data-ttu-id="0fbca-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0fbca-135">Not yet documented</span></span>|
|<span data-ttu-id="0fbca-136">userId</span><span class="sxs-lookup"><span data-stu-id="0fbca-136">userId</span></span>|<span data-ttu-id="0fbca-137">Guid</span><span class="sxs-lookup"><span data-stu-id="0fbca-137">Guid</span></span>|<span data-ttu-id="0fbca-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0fbca-138">Not yet documented</span></span>|
|<span data-ttu-id="0fbca-139">отпечаток</span><span class="sxs-lookup"><span data-stu-id="0fbca-139">thumbprint</span></span>|<span data-ttu-id="0fbca-140">String</span><span class="sxs-lookup"><span data-stu-id="0fbca-140">String</span></span>|<span data-ttu-id="0fbca-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0fbca-141">Not yet documented</span></span>|
|<span data-ttu-id="0fbca-142">усерупн</span><span class="sxs-lookup"><span data-stu-id="0fbca-142">userUpn</span></span>|<span data-ttu-id="0fbca-143">String</span><span class="sxs-lookup"><span data-stu-id="0fbca-143">String</span></span>|<span data-ttu-id="0fbca-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0fbca-144">Not yet documented</span></span>|
|<span data-ttu-id="0fbca-145">енкриптедпфксблоб</span><span class="sxs-lookup"><span data-stu-id="0fbca-145">encryptedPfxBlob</span></span>|<span data-ttu-id="0fbca-146">String</span><span class="sxs-lookup"><span data-stu-id="0fbca-146">String</span></span>|<span data-ttu-id="0fbca-147">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0fbca-147">Not yet documented</span></span>|
|<span data-ttu-id="0fbca-148">енкриптедпфкспассворд</span><span class="sxs-lookup"><span data-stu-id="0fbca-148">encryptedPfxPassword</span></span>|<span data-ttu-id="0fbca-149">String</span><span class="sxs-lookup"><span data-stu-id="0fbca-149">String</span></span>|<span data-ttu-id="0fbca-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0fbca-150">Not yet documented</span></span>|
|<span data-ttu-id="0fbca-151">цертстартдате</span><span class="sxs-lookup"><span data-stu-id="0fbca-151">certStartDate</span></span>|<span data-ttu-id="0fbca-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fbca-152">DateTimeOffset</span></span>|<span data-ttu-id="0fbca-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0fbca-153">Not yet documented</span></span>|
|<span data-ttu-id="0fbca-154">цертекспиратиондате</span><span class="sxs-lookup"><span data-stu-id="0fbca-154">certExpirationDate</span></span>|<span data-ttu-id="0fbca-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fbca-155">DateTimeOffset</span></span>|<span data-ttu-id="0fbca-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0fbca-156">Not yet documented</span></span>|
|<span data-ttu-id="0fbca-157">providerName</span><span class="sxs-lookup"><span data-stu-id="0fbca-157">providerName</span></span>|<span data-ttu-id="0fbca-158">String</span><span class="sxs-lookup"><span data-stu-id="0fbca-158">String</span></span>|<span data-ttu-id="0fbca-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0fbca-159">Not yet documented</span></span>|
|<span data-ttu-id="0fbca-160">енкриптионкэйнаме</span><span class="sxs-lookup"><span data-stu-id="0fbca-160">encryptionKeyName</span></span>|<span data-ttu-id="0fbca-161">String</span><span class="sxs-lookup"><span data-stu-id="0fbca-161">String</span></span>|<span data-ttu-id="0fbca-162">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0fbca-162">Not yet documented</span></span>|
|<span data-ttu-id="0fbca-163">паддингсчеме</span><span class="sxs-lookup"><span data-stu-id="0fbca-163">paddingScheme</span></span>|<span data-ttu-id="0fbca-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0fbca-164">Int32</span></span>|<span data-ttu-id="0fbca-165">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0fbca-165">Not yet documented</span></span>|
|<span data-ttu-id="0fbca-166">status</span><span class="sxs-lookup"><span data-stu-id="0fbca-166">status</span></span>|<span data-ttu-id="0fbca-167">Int32</span><span class="sxs-lookup"><span data-stu-id="0fbca-167">Int32</span></span>|<span data-ttu-id="0fbca-168">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0fbca-168">Not yet documented</span></span>|
|<span data-ttu-id="0fbca-169">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="0fbca-169">intendedPurpose</span></span>|<span data-ttu-id="0fbca-170">Int32</span><span class="sxs-lookup"><span data-stu-id="0fbca-170">Int32</span></span>|<span data-ttu-id="0fbca-171">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0fbca-171">Not yet documented</span></span>|
|<span data-ttu-id="0fbca-172">createdTime</span><span class="sxs-lookup"><span data-stu-id="0fbca-172">createdTime</span></span>|<span data-ttu-id="0fbca-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fbca-173">DateTimeOffset</span></span>|<span data-ttu-id="0fbca-174">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0fbca-174">Not yet documented</span></span>|
|<span data-ttu-id="0fbca-175">isDeleted</span><span class="sxs-lookup"><span data-stu-id="0fbca-175">isDeleted</span></span>|<span data-ttu-id="0fbca-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fbca-176">Boolean</span></span>|<span data-ttu-id="0fbca-177">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0fbca-177">Not yet documented</span></span>|
|<span data-ttu-id="0fbca-178">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="0fbca-178">lastModifiedTime</span></span>|<span data-ttu-id="0fbca-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fbca-179">DateTimeOffset</span></span>|<span data-ttu-id="0fbca-180">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0fbca-180">Not yet documented</span></span>|
|<span data-ttu-id="0fbca-181">eTag</span><span class="sxs-lookup"><span data-stu-id="0fbca-181">eTag</span></span>|<span data-ttu-id="0fbca-182">String</span><span class="sxs-lookup"><span data-stu-id="0fbca-182">String</span></span>|<span data-ttu-id="0fbca-183">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0fbca-183">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0fbca-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="0fbca-184">Response</span></span>
<span data-ttu-id="0fbca-185">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0fbca-185">If successful, this method returns a `201 Created` response code and a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fbca-186">Пример</span><span class="sxs-lookup"><span data-stu-id="0fbca-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fbca-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fbca-187">Request</span></span>
<span data-ttu-id="0fbca-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0fbca-188">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0fbca-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fbca-189">Response</span></span>
<span data-ttu-id="0fbca-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0fbca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






